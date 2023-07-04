# Product Endpoint

The Product endpoint allows you to manage products in your application.

## Get Products

If `modelo ` isn't set retrieves a list of all products, if it's set it retrieves only the product matching the modelo.

-   Method: GET
-   Endpoint: `/product?modelo=product_modelo`
-   admin level: `0`
-   URL Parameters:
    -   `modelo` (optional): Product modelo

## Create Product

Creates a new product.

-   Method: POST
-   Endpoint: `/product`
-   admin level: `1`
-   Required Parameters:
    -   `modelo`: Name of the product
    -   `price`: Price of the product
    -   `description`: Description of the product
    -   `categoria` : Category of the product (should be already created)

## Update Product

Updates an existing product.

-   Method: PATCH
-   Endpoint: `/product/{id}`
-   admin level: `1`
-   Required Parameters:
    -   `id`: ID of the product to update
    -   `modelo` (optional): New name for the product
    -   `price` (optional): New price for the product
    -   `description` (optional): New description for the product

## Delete Product

Deletes a product.

-   Method: DELETE
-   Endpoint: `/product/{id}`
-   admin level: `1`
-   Required Parameters:
    -   `id`: ID of the product to delete
