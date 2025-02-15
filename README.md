# Product API - Simple Web Server

## What This Project Does

- Runs a web server using **Express.js**.
- Provides a list of products.
- Filters products by category using query parameters.
- Fetches product details by ID.

## How to Use

1. **Install Node.js** if you don’t have it.
2. Open the project folder in a terminal.
3. Install Express:
   ```sh
   npm install express
   ```
4. Start the server:
   ```sh
   node server.js
   ```
5. Open `http://localhost:3000/products` in your browser to see all products.
6. Add `?category=electronics` or `?category=fashion` to filter by category.
7. Open `http://localhost:3000/products/1` (replace `1` with any product ID) to view product details.

## How It Works

| Route               | What It Does                           |
|---------------------|--------------------------------------|
| `/products`        | Shows all products                   |
| `/products?category=electronics` | Filters by category (e.g., electronics, fashion) |
| `/products/:id`    | Fetches product details by ID        |

## Example Product Data

```json
[
  {
    "id": 1,
    "name": "Laptop",
    "category": "electronics",
    "price": 1200
  },
  {
    "id": 2,
    "name": "Phone",
    "category": "electronics",
    "price": 800
  }
]
```

## Project Files

```
/project-folder
│-- server.js      # Runs the server
│-- package.json   # Dependencies
│-- README.mdn     # This file
```

## Notes

- The server runs on **PORT 3000**.
- If a product ID does not exist, it returns a `404 Not Found` error.

That's it! 🎉

