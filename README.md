# Funiture API

## API documentation

This API only supports GET requests.

### Return all product categories

* **URL**

  /categories

* **Method:**

  `GET`

* **URL Params**

   There are no URL params

  **Example:**

  `/categories`

* **Success Response:**

    * **Code:** 200 <br />
      **Content:** <br />

  ```json
  {
    "message": "Successfully retrieved categories",
    "data":
    [
        {
            "id": "1",
            "name": "Chair",
            "products": "82"
        },
        {
            "id": "2",
            "name": "Table",
            "products": "37"
        }
    ]
  }
  ```

* **Error Response:**

    * **Code:** 500 SERVER ERROR <br />
      **Content:** `{"message": "Unexpected error", "data": []}`
