**Accommodation Model**
----

  ```json
    {
      "id": "Integer",
      "category": "Accommodation",
      "name": "String",
      "address": "String",
      "address2": "String",
      "city": "String",
      "province": "String",
      "country": "String",
      "postalcode": "String",
      "categories": [
        {
          "code": "String", 
          "name": "String",
          "min": "Integer",
          "max": "Integer",
          "pricing": ["PP", "PS"]
        },
      ],
      "sell_date_breaks": [
        {
          "start": "DateTime",
          "end": "DateTime",
          "days": {
            "mon": "boolean",
            "tue": "boolean",
            "wed": "boolean",
            "thu": "boolean",
            "fri": "boolean",
            "sat": "boolean",
            "sun": "boolean"
          },
          "categories": [
            {
              "amount": "Float",
              "min": "Integer",
              "max": "Integer",
              "code": "String"
            }
          ]
        },
      ],
      "cost_date_breaks": [
        {
          "start": "DateTime",
          "end": "DateTime",
          "days": {
            "mon": "boolean",
            "tue": "boolean",
            "wed": "boolean",
            "thu": "boolean",
            "fri": "boolean",
            "sat": "boolean",
            "sun": "boolean"
          },
          "categories": [
            {
              "amount": "Float",
              "min": "Integer",
              "max": "Integer",
              "code": "String"
            }
          ]
        },
      ]
    }
  ```
