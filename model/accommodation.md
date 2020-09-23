**Accommodation Model**
----

  ```json
    {
      "id": "Integer",
      "category": "Accommodation",
      "name": "String",
      "description": "String",
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
            "mon": "Boolean",
            "tue": "Boolean",
            "wed": "Boolean",
            "thu": "Boolean",
            "fri": "Boolean",
            "sat": "Boolean",
            "sun": "Boolean"
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
            "mon": "Boolean",
            "tue": "Boolean",
            "wed": "Boolean",
            "thu": "Boolean",
            "fri": "Boolean",
            "sat": "Boolean",
            "sun": "Boolean"
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
      "minimum_nights_breaks": [
        {
          "start": "DateTime",
          "end": "DateTime",
          "min": "Integer",
          "max": "Integer",
          "pricing": ["PP", "PS"]
        },
      ],
      "terms": "String"
    }
  ```
