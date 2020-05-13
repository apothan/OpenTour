**ProductDetail**
----
  Returns json data about a single product.

* **URL**

  /api/productdetail.json

* **Method:**

  `POST`

* **Data Params**

  None
  
* **Sample Request:**

  ```json
    {
      "username": "username",
      "token": "password",
      "productid": "11"
    }
  ```

* **Success Response:**

  ```json
    {
      "productid": 11,
      "name": "Tour of Italy",
      "family": "Tour",
      "duration": 9,
      "lat": "0.000000",
      "lng": "0.000000",
      "country": "IT",
      "city": "Rome",
      "tourdate": "2020-09-01T00:00:00-04:00",
      "sellcurrency": "USD",
      "symbol": "US$",
      "categories": [
        {
          "id": 11,
          "itemid": 11,
          "category": "Single",
          "catshort": "SGL",
          "min": 1,
          "max": 1,
          "star": "0",
          "pricing": "PP"
        },
        {
          "id": 12,
          "itemid": 11,
          "category": "Double",
          "catshort": "DBL",
          "min": 2,
          "max": 2,
          "star": "0",
          "pricing": "PP"
        },
        {
          "id": 15,
          "itemid": 11,
          "category": "Triple",
          "catshort": "TPL",
          "min": 3,
          "max": 3,
          "star": "0",
          "pricing": "PP"
        }
      ],  
      "totalcats": 3,
      "breaks": [
        {
          "start": "2020-09-01T00:00:00-04:00",
          "end": "2020-09-01T00:00:00-04:00",
          "duration": 9,
          "days": {
            "mon": true,
            "tue": true,
            "wed": true,
            "thu": true,
            "fri": true,
            "sat": true,
            "sun": true 
          },
          "amounts": [
            {
              "amount": "5919.00",
              "min": 1,
              "max": 1,
              "categoryid": 11,
              "category": "Single"
            },
            {
              "amount": "4499.00",
              "min": 2,
              "max": 2,
              "categoryid": 12,
              "category": "Double"
            },
            {
              "amount": "4499.00",
              "min": 3,
              "max": 3,
              "categoryid": 15,
              "category": "Triple"
            }
          ],
        }
      ],
      "included": [],
      "coordinates": [],
      "features": [],
      "low": "3499.00"
    }
  ```
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
    **Content:** `{ error : "No product returned!" }`

  OR

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`


