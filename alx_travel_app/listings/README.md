📘 alx_travel_app_0x01
Objective

This project implements API views for Listings and Bookings using Django REST Framework.
It provides full CRUD operations and exposes endpoints under /api/ with Swagger documentation.

🛠 Features

Listings API – create, view, update, delete travel listings.

Bookings API – create, view, update, delete bookings for listings.

RESTful endpoints with Django REST Framework.

Swagger/OpenAPI docs for interactive testing.

📂 Project Structure
alx_travel_app_0x01/
│── alx_travel_app/
│   ├── settings.py
│   ├── urls.py
│── listings/
│   ├── models.py
│   ├── views.py   # API ViewSets
│   ├── urls.py    # Router endpoints
│── manage.py
└── README.md

⚙️ Setup Instructions

Clone the repository

git clone https://github.com/<your-username>/alx_travel_app_0x01.git
cd alx_travel_app_0x01


Create & activate a virtual environment

python3 -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate


Install dependencies

pip install -r requirements.txt


Run migrations

python manage.py makemigrations
python manage.py migrate


Start the development server

python manage.py runserver

🚀 API Endpoints

Base URL: http://127.0.0.1:8000/api/

Endpoint	Method	Description
/api/listings/	GET	Get all listings
/api/listings/	POST	Create new listing
/api/listings/{id}/	GET	Get listing by ID
/api/listings/{id}/	PUT	Update listing by ID
/api/listings/{id}/	DELETE	Delete listing by ID
/api/bookings/	GET	Get all bookings
/api/bookings/	POST	Create new booking
/api/bookings/{id}/	GET	Get booking by ID
/api/bookings/{id}/	PUT	Update booking by ID
/api/bookings/{id}/	DELETE	Delete booking by ID
📖 API Documentation

Swagger UI: http://127.0.0.1:8000/swagger/

ReDoc: http://127.0.0.1:8000/redoc/

✅ Testing

Use Postman or curl to test endpoints. Example:

curl -X POST http://127.0.0.1:8000/api/listings/ \
  -H "Content-Type: application/json" \
  -d '{"title": "Beach Resort", "description": "A nice place to relax"}'

👨‍💻 Author

Project by Samuel Adikah – ALX Backend Development
