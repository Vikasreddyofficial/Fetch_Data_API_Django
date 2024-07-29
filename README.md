
# Emp_DATA Django Project
## Overview

The Emp_DATA Django project is a web application that allows users to upload CSV files and query the data. It includes a REST API for uploading CSV files and retrieving filtered data. The project uses Django 4.2.13 and PostgreSQL as the database backend.g.

# Features
- CSV Upload: Upload CSV files containing educational data.
- Data Query: Filter and retrieve data based on various query parameters.
- API Documentation: Automatically generated Swagger and Redoc documentation for the API endpoints.


# Installation

1. Clone the repository:

```bash
  git clone https://github.com/Vikasreddyofficial/Fetch_Data_API_Django.git
  cd Fetch_Data_API_Django
```
2. Create and activate a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate 

```
3. Install Dependencies

```bash
pip install -r requirements.txt

```
4. Set up the PostgreSQL database:

- Ensure you have PostgreSQL installed and running.

5. Apply the migrations:

```bash
python manage.py migrate

```
6. Run the development server:

```bash
python manage.py runserver

```

# Configuration

## API Documentation:

- Swagger UI: http://127.0.0.1:8000/swagger/
- ReDoc UI: http://127.0.0.1:8000/redoc/


## API Endpoints
Here's a list of available API endpoints in the project:

1. Upload CSV:

- URL: /api/upload_csv/
- Method: POST
- Description: Upload a CSV file to the server. The file must be in CSV format.
- Parameters:  file - The CSV file to upload.

2. Get Filtered Data

- URL: /api/get_filtered_data/
- Method: GET
- Description: Retrieve data filtered by ac_year and state_name. Optionally limit the number of rows returned.
- Parameters:
  - ac_year: Filter data by academic year.
  - state_name: Filter data by state name.
  - limit: Limit the number of rows returned.


## Dependencies
The project requires the following packages:
- Django==4.2.13
- djangorestframework
- drf_yasg
- psycopg2-binary # PostgreSQL adapter for Python
For the full list of dependencies, refer to the requirements.txt file.

## Contributing
Contributions are welcome! Fork the repository, make your changes, and submit a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details