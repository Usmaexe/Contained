# Contained

Contained is a repository containing a Dockerized Django application with features for handling Client Requests to chat-gpt the gpt-3.5 model is used since text-davinci-003 is deprecated..


## Prerequisites

Make sure you have Docker Desktop Running on your local machine 

## Getting Started

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/Contained.git
    cd Contained
    git ChatGptApi update --init --recursive
    ```

2. Build and run the Docker containers:

    ```bash
    docker-compose up -d --build
    ```

3. Access the Django application:

    Open your web browser and go to [http://localhost:8089/](http://localhost:8089/)


## Directory Structure

- `ChatGptApi/`: Contains Django application source code, templates and the endpoint 
- `venv/`: Virtual environment for Python dependencies
- `docker-compose.yml`: Docker Compose configuration file
- `Dockerfile`: Dockerfile for building the Docker image
- `requirements.txt`: Located in ChatGptApi it is a List of Python dependencies

## Docker Compose Configuration

The `docker-compose.yml` file is configured to mount the `ChatGptApi` directory as the source code for the Django application and expose the necessary ports. 

It also maps the `Content.csv` file from the host to the container.

## Notes

- The application will be accessible at [http://localhost:8089/](http://localhost:8089/)
- The CSV file is stored in the `ChatGptApi/data/` directory in the container.
- This project is actively maintained and will be updated in the future to incorporate improvements and additional features.


