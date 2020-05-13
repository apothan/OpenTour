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
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
    **Content:** `{ error : "No products returned!" }`

  OR

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`


