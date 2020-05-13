**BookingCreate**
----
  Books the requested product and returns booking details.

* **URL**

  /api/bookingcreate.json

* **Method:**

  `POST`

* **Data Params**

  None
  
* **Sample Request:**

  ```json
    {
      "username": "username",
      "token": "password",
      "customer": {
        "email": "string",
        "phone": "1234567890",
        "address1": "string",
        "address2": "string",
        "city": "string",
        "province": "string",
        "country": "string",
        "postalcode": "string"
      },
      "note": "string",
      "depdate": "2018-08-31",
      "products": [
        {
          "catid": "378",
          "depdate": "2018-08-31",
          "servicedate": "2018-08-31",
          "duration": "1",
          "quantity": "1",
          "passengers": [
            {
              "title": "Mr",
              "firstname": "John",
              "surname": "Smith",
              "dob": "1985-01-01"
            }
          ]
        }
      ],
      "payment": {
        "paymentamount": "200",
        "paymentmethod": "Visa, MasterCard, Amex",
        "cardholdername": "John Smith",
        "cardnumber": "5105105105105100",
        "cardcvv": "123",
        "cardexpmonth": "06",
        "cardexpyear": "2019",
        "cardaddress": "123 hello st",
        "cardcity": "City",
        "cardcountry": "Country"
      }
    }
  ```

* **Success Response:**

  ```json
    {
      "id": "54139",
      "customer": "16925",
      "date": "2018-08-20T18:47:43+00:00",
      "depdate": "2018-08-31T00:00:00+00:00",
      "terms": "These are the company terms & conditions.",
      "passengers": [
        {
          "title": "Mr",
          "firstname": "John",
          "surname": "Smith",
          "dob": "1985-01-01"
        }
      ],
      "invoiceitems": [
        {
          "quantity": "1",
          "description": "View from the Shard | Adult",
          "amount": "0",
          "date": "2018-08-31T00:00:00+00:00",
          "enddate": "2018-09-01T00:00:00+00:00",
          "duration": "1",
          "passengers": [
            {
              "title": "Mr",
              "firstname": "John",
              "surname": "Smith",
              "dob": "1985-01-01"
            }
          ]
        }
      ],
      "sellcurrency": "USD",
      "totalpayment": "200.00",
      "balance": "-200.00",
      "netbalance": "-200.00",
      "commission": "0",
      "total": "0",
      "subtotal": "0",
      "bookingnumber": "54139"
    }
  ```
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`


