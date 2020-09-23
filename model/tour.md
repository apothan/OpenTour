**Tour Model**
----

  ```json
    {
      "id": "Integer",
      "category": "Tour",
      "name": "String",
      "description": "String",
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
      "itinerary": [
        {
          "header": "String",
          "description": "String"
        },
      ],
      "features": [
        {
          "description": "String"
        },
      ],
      "coordinates": [
        {
          "coorx": "Float",
          "coory": "Float",
          "city": "String"
        }
      ],
      "terms": "String"
    }
  ```
