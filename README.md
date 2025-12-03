# Giulia Handmade Assets

This repository hosts all static assets for the Giulia Handmade website.

## Folder Structure

- **`/logo/`**: Contains the brand logo files.
- **`/products/`**:
    - **`/web/`**: Optimized images for the website (.jpg, .webp). Use these in `products.json`.
    - **`/originals/`**: High-resolution original photos (for backup/future use).
    
    > **Note:** The current sample images are `.svg` placeholders. When you add real product images, please use `.jpg` or `.webp` formats and update `products.json` accordingly.

- **`/icons/`**: Social media icons and other UI elements.
- **`/json/`**: Data files defining content.

## How to Add a New Product

1.  **Prepare Images**:
    - Rename your images clearly, e.g., `my-new-bag-01.jpg`.
    - Place optimized versions in `products/web/`.
    - Place original high-res versions in `products/originals/` (optional but recommended).

2.  **Update `products.json`**:
    - Open `json/products.json`.
    - Add a new entry to the list following this format:

    ```json
    {
      "id": "unique-id-001",
      "name": "Product Name",
      "category": "Category",
      "images": [
        "products/web/my-new-bag-01.jpg",
        "products/web/my-new-bag-02.jpg"
      ],
      "description": "Description of the product."
    }
    ```

3.  **Commit & Push**:
    - If using GitHub Desktop or web interface, commit your changes and push to the repository. The website will update automatically (if configured to fetch this JSON).
