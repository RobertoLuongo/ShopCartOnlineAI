# Auto Parts Shop Cart

This is a shop cart application for automobile parts with a Node.js backend and Angular frontend.

## Project Structure

- `/automobileParts.json` - The data source for automobile parts
- `/backend` - Express.js backend API
- `/frontend` - Angular frontend application

## Features

- REST API with methods to get automobile parts, search, and filter
- Product listing page with pagination
- Product detail page
- Search functionality by name, description, manufacturer
- Price range filter
- Shopping cart with add/remove functionality
- Cart total calculation

## Running the Application

### Backend

1. Navigate to the backend directory:

   ```
   cd backend
   ```

2. Install dependencies:

   ```
   npm install
   ```

3. Start the server:
   ```
   npm run dev
   ```

The backend will start on http://localhost:3000

### Frontend

1. Navigate to the frontend directory:

   ```
   cd frontend
   ```

2. Install dependencies:

   ```
   npm install
   ```

3. Start the Angular development server:
   ```
   ng serve
   ```

The frontend will start on http://localhost:4200

## API Endpoints

- `GET /api/parts?page=0&limit=10` - Get paginated list of automobile parts
- `GET /api/parts/:id` - Get automobile part details by ID
- `GET /api/search` - Search automobile parts with parameters:
  - `name` - Filter by name
  - `description` - Filter by description
  - `manufacturer` - Filter by manufacturer
  - `minPrice` - Filter by minimum price
  - `maxPrice` - Filter by maximum price

## Technologies Used

- Backend:
  - Node.js
  - Express.js
- Frontend:
  - Angular
  - Bootstrap

## Future Enhancements

- User authentication
- Order processing
- Payment integration
- Admin dashboard for product management
