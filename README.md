# Funiture API

## API documentation

This API only supports GET requests.

### Return all product categories

* **URL**

  /categories.php

* **Method:**

  `GET`

* **URL Params**

   There are no URL params

  **Example:**

  `/categories.php`

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

### Return all products in a category

* **URL**

  /products.php

* **Method:**

  `GET`

* **URL Params**

   **Required:**
   
   `cat` - category ID for the required products

  **Example:**

  `/products.php?cat=2`

* **Success Response:**

    * **Code:** 200 <br />
      **Content:** <br />

  ```json
  {
    "message": "Successfully retrieved products",
    "data":
    [
        {
          "price": "48.61",
          "stock": 8,
          "color": "Teal"
        },
        {
          "price": "182.08",
          "stock": 2,
          "color": "Green"
        }
    ]
  }
  ```

* **Error Response:**

    * **Code:** 500 SERVER ERROR <br />
      **Content:** `{"message": "Unexpected error", "data": []}`
