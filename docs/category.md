# Category Endpoint

The Category endpoint allows you to manage categories.

## Get Categories

If `titulo` isn't set retrieves a list of all categories, if it's set it retrieves only the category matching the title.

- Method: GET
- Endpoint: `/category?titulo="titulo"`
- admin level: `0`
- URL Parameters:
    - `titulo` (optional): Title of the category

## Create Category

Creates a new category.

- Method: POST
- Endpoint: `/category`
- admin level: `1`
- Parameters:
    - `titulo`  : Title of the category
    - `descripcion`  : Description of the category
    - `imagen`  : Image URL of the category

## Update Category

Updates an existing category.

- Method: PATCH
- Endpoint: `/category`
- admin level: `1`
- Parameters:
    - `id`  : ID of the category to update
    - `titulo` (optional): New title for the category
    - `descripcion` (optional): New description for the category
    - `imagen` (optional): New image URL for the category

## Delete Category

Deletes a category.

- Method: DELETE
- Endpoint: `/category`
- admin level: `1`
- Parameters:
    - `id`  : ID of the category to delete
