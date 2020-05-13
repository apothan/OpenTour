**ProductSearch**
----
  Returns json data about available products based upon query.

* **URL**

  /api/productsearch.json

* **Method:**

  `POST`

* **Data Params**

  None
  
* **Sample Request:**

  ```json
    {
      "username": "username",
      "token": "password",
      "servicerequest": {
        "category": "Tour"
      },
      "hidepricing": false,
      "start": 0,
      "records": 10
    }
  ```

* **Success Response:**

  ```json
    {
      "products": {
        11: {
          "productid": 11,
          "category": "Tour",
          "servicename": "Tour oF Italy",
          "city": "YYZ",
          "tourdate": "2021-01-29T00:00:00-05:00",
          "duration": 12,
          "quantity": 1,
          "lowsell": "3519.00"
        },
      "terms": "Your terms and conditions",
      "rows": 1
    }
  ```
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
    **Content:** `{ error : "No products returned!" }`

  OR

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`


