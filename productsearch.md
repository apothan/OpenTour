**ProductSearch**
----
  Returns json data about available products based upon query.

* **URL**

  /api/productsearch.json

* **Method:**

  `POST`

* **Data Params**

  username=[string] <br />
  token=[string] <br />
  category=['Tour','Accommodation','Excursion','Transfer','CarRental','Air','Insurance'] <br />
  start=[integer] <br />
  records=[integer]
  
* **Sample Request:**

  ```json
    {
      "username": "username",
      "token": "password",
      "servicerequest": {
        "category": "Tour"
      },
      "start": 0,
      "records": 10
    }
  ```

* **Success Response:**

  ```json
    {
      "products": [
        {
          "id": 11,
          "category": "Tour",
          "name": "Tour of Italy",
          "city": "Rome",
          "tourdate": "2021-01-29T00:00:00-05:00",
          "nights": 12
        }
      ],
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


