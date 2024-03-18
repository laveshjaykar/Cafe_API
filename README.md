# Cafe_API

This repository contains a simple Flask application that simulates a Cafe API. The API provides endpoints for managing a list of cafes, including creating, reading, updating, and deleting cafe records from a SQLite database.

Features

SQLite Database Integration: Utilizes Flask_SQLAlchemy for ORM and SQLite for data storage.
CRUD Operations: Supports Create, Read, Update, and Delete operations for cafe data.
Random Cafe Endpoint: Fetches a random cafe from the database.
Search Functionality: Allows searching for cafes by location.
Data Validation and Error Handling: Implements basic validation and error handling for API requests.

Endpoints

GET /: The home route that serves the index.html page.
GET /random: Returns a random cafe from the database in JSON format.
GET /all: Retrieves all cafes from the database in JSON format.
GET /search: Searches for cafes by location. Requires a query parameter loc indicating the desired location.
POST /add: Adds a new cafe to the database. Requires form data with cafe details.
PATCH /update-price/<int:cafe_id>: Updates the coffee price for a specific cafe. Requires the new price as a query parameter new_price.
DELETE /report-closed/<int:cafe_id>: Deletes a cafe from the database. Requires an api-key query parameter for authentication.
