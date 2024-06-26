## Features
- Connect with OpenAI GPT-3.5 language model for conversation
- Employ OpenAI's text-embedding-ada-002 for text embedding
- Python Langchain library for file processing and text c
- Multilingual support
- AWS S3 bucket support for scalable hosting
- Easy deployment on Heroku or AWS

## How to run

- Clone the repository. `git clone https://github.com/shamspias/customizable-gpt-chatbot`
- Install the required packages by running `pip install -r requirements.txt`
- Run celery `celery -A config worker --loglevel=info`
- Run the command `python manage.py runserver`
- Open `http://127.0.0.1:8000/` in your browser

In linux and mac need to install 'sudo apt install python3-dev -y`

1. Make sure that you have the development libraries for libcurl installed on your system. You can install them by running the following command: `sudo apt-get install libcurl4-openssl-dev gcc libssl-dev -y`
2. Make sure that you have the latest version of pip and setuptools installed by running the following command: `pip install --upgrade pip setuptools`
3. `pip install pycurl`

## Deployment

The chatbot can be deployed on Heroku or AWS by following the standard procedures for Django deployment on these platforms.

## Issues

- If you don't use AWS SQS then no need to install `pycurl` and `boto3` packages.
- If you don't use AWS S3 then no need to install `django-storages` package.

## Note

Make sure that you have API key from OpenAI before running the project.
Enjoy!
