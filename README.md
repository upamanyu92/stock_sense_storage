# Database Microservice

This microservice provides RESTful APIs for managing stock quotes and predictions. 

## Features

- CRUD operations for stock quotes
- CRUD operations for predictions
- Health check endpoint
- SQLAlchemy ORM
- Alembic for database migrations
- Dockerized

## Setup

1. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

2. Run migrations:

    ```bash
    flask db upgrade
    ```

3. Start the application:

    ```bash
    python run.py
    ```

4. Run with Docker:

    ```bash
    docker build -t db_microservice .
    docker run -p 5000:5000 db_microservice
    ```

## Endpoints

- `/api/stock_quotes/`: CRUD operations for stock quotes.
- `/api/predictions/`: CRUD operations for predictions.
- `/api/health_check/`: Health check endpoint.
