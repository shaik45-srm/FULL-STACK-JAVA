

# Product List

This repository contains a collection of product data, represented as JavaScript objects. Each product includes details such as name, image, rating, price, and relevant keywords.

## Product Structure

Each product object contains the following fields:

- **id**: A unique identifier for the product (UUID format).
- **image**: The path to the product image (relative to the root directory).
- **name**: The name of the product.
- **rating**: An object containing:
  - **stars**: Average product rating (out of 5).
  - **count**: Number of ratings the product has received.
- **priceCents**: The price of the product in cents (used to avoid floating-point imprecision).
- **keywords**: An array of strings representing relevant search keywords for the product.
- **type** (optional): The type/category of the product (e.g., "clothing").
- **sizeChartLink** (optional): A link to the size chart image, used for clothing products.

## Example of a Product Object

```js
{
  id: "e43638ce-6aa0-4b85-b27f-e1d07eb678c6",
  image: "images/products/athletic-cotton-socks-6-pairs.jpg",
  name: "Black and Gray Athletic Cotton Socks - 6 Pairs",
  rating: {
    stars: 4.5,
    count: 87
  },
  priceCents: 1090,
  keywords: [
    "socks",
    "sports",
    "apparel"
  ]
}
```

### Sample Products

1. **Black and Gray Athletic Cotton Socks - 6 Pairs**
   - **Rating**: 4.5 stars (87 reviews)
   - **Price**: $10.90
   - **Keywords**: socks, sports, apparel
   - **Image**: ![Image](images/products/athletic-cotton-socks-6-pairs.jpg)

2. **Intermediate Size Basketball**
   - **Rating**: 4 stars (127 reviews)
   - **Price**: $20.95
   - **Keywords**: sports, basketballs
   - **Image**: ![Image](images/products/intermediate-composite-basketball.jpg)

3. **2 Slot Toaster - Black**
   - **Rating**: 5 stars (2,197 reviews)
   - **Price**: $18.99
   - **Keywords**: toaster, kitchen, appliances
   - **Image**: ![Image](images/products/black-2-slot-toaster.jpg)

4. **Liquid Laundry Detergent, 110 Loads, 82.5 Fl Oz**
   - **Rating**: 4.5 stars (305 reviews)
   - **Price**: $28.99
   - **Keywords**: bathroom, cleaning
   - **Image**: ![Image](images/products/liquid-laundry-detergent-plain.jpg)

## How to Use

You can use this product data to display products on an e-commerce website or in any other application requiring product information.

1. **Import the Product Data:**
   - Copy the `products` array and import it into your JavaScript application.

2. **Filter Products by Category/Keyword:**
   - Use the `keywords` array to filter products by category (e.g., "shoes", "sports", etc.).

3. **Display Product Information:**
   - Loop through the `products` array and dynamically display product names, ratings, images, and prices on your website or in an app.

4. **Price Conversion:**
   - Convert `priceCents` to a more user-friendly format using simple math:
     ```js
     const priceInDollars = product.priceCents / 100;
     ```

## License

This product data is shared under the [MIT License](LICENSE).

---

