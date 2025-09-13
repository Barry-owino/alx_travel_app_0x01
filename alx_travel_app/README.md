ALX Travel App – API

This project is part of the ALX Backend Specialization.
It extends the alx_travel_app_0x00 project into alx_travel_app_0x01 by adding API endpoints for managing listings and bookings, with documentation using Swagger.

Features

CRUD operations for Listings and Bookings.

RESTful API built using Django REST Framework.

Interactive API documentation using Swagger UI.

Tested endpoints with cURL and Postman.

Installation & Setup

Clone the repository:

git clone https://github.com/<your-username>/alx_travel_app_0x01.git
cd alx_travel_app_0x01


Create virtual environment & activate:

python3 -m venv myworld
source myworld/bin/activate


Install dependencies:

pip install -r requirements.txt


Apply migrations:

python manage.py migrate


Run the server:

python manage.py runserver

API Endpoints
Listings

GET /api/listings/ → Get all listings

POST /api/listings/ → Create a new listing

GET /api/listings/{id}/ → Retrieve a listing by ID

PUT /api/listings/{id}/ → Update a listing by ID

DELETE /api/listings/{id}/ → Delete a listing by ID

Bookings

GET /api/bookings/ → Get all bookings

POST /api/bookings/ → Create a new booking

GET /api/bookings/{id}/ → Retrieve a booking by ID

PUT /api/bookings/{id}/ → Update a booking by ID

DELETE /api/bookings/{id}/ → Delete a booking by ID

Testing the API
Using cURL
# Create a new listing
curl -X POST http://127.0.0.1:8000/api/listings/ \
-H "Content-Type: application/json" \
-d '{"title":"City Aparto","description":"Modern shipping containers","price":50000.00,"location":"Nairobi"}'

# Get all listings
curl -X GET http://127.0.0.1:8000/api/listings/

Using Postman

Import the endpoints into a collection.

Test GET, POST, PUT, DELETE with JSON payloads.

API Documentation

Interactive docs are available with Swagger and ReDoc:

Swagger UI → http://127.0.0.1:8000/swagger/

ReDoc → http://127.0.0.1:8000/redoc/

Repository Structure
alx_travel_app_0x01/
│── alx_travel_app/        # Main Django project
│   └── settings.py
│   └── urls.py
│── listings/              # Listings app
│   └── models.py
│   └── views.py
│   └── serializers.py
│   └── urls.py
│── manage.py
│── README.md

Author

👨‍💻 Barry Owino
Software Engineer | Backend Developer (Python/Django)
