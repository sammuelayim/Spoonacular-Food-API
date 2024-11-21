# Spoonacular-Food-API
The main objective is to practice working with APIs by customizing requests, extracting structured data, and visualizing it.
# Spoonacular Recipe Analysis

## Project Overview
This project demonstrates how to interact with the [Spoonacular Food API](https://spoonacular.com/food-api) to retrieve and analyze recipe data. By leveraging this API, we fetch information about various recipes based on user-defined queries and analyze the data to generate useful insights.

The main objective is to practice working with APIs by customizing requests, extracting structured data, and visualizing it.

---

## API Details
The [Spoonacular Food API](https://spoonacular.com/food-api) provides access to a wide range of food-related data, including recipes, ingredients, nutrition facts, and more.

### Key Features Used:
1. **Recipe Search**:
   - **Endpoint**: `/recipes/complexSearch`
   - Fetches a list of recipes based on a search query (e.g., "pizza," "smoothie").
   - Returns data such as `id`, `title`, and `image`.

2. **Recipe Information**:
   - **Endpoint**: `/recipes/{id}/information`
   - Provides detailed information about a recipe using its unique ID.
   - Includes fields like `servings`, `readyInMinutes`, `sourceUrl`, and `ingredients`.

### Authentication:
- Requires an API key, included as a query parameter (`apiKey`) in all requests.

### Parameters Used:
- **`query`**: The keyword to search for recipes (e.g., "pasta").
- **`number`**: Number of results to return.
- **`includeNutrition`**: Boolean to include nutritional data (optional).
- **`apiKey`**: Your Spoonacular API key.

Example API Call:
```url
https://api.spoonacular.com/recipes/complexSearch?query=pizza&number=5&apiKey=5ca0c0715f32487d87a470effcd8d8f5
