# deutsche-bahn
A prototype service to explore how RESTful APls can enhance experience of passengers around Germany.

This API extracts relevant data from the Deutsche Bahn (German high speed train network) database and uses Google Gemini to create a tourism guide. The API contains the following features, all polished with endpoints and swaggerdoc adhering to RESTful API Design guidelines.This Data Service stores all data in an SQLite database, querying when necessary.

Access the Swagger OpenAPI docs here: [link TBA]

## Setup

To run the app locally, first create a fork of the repository and clone it.

Then, use `pip3 install` to install the following libraries:
- dotenv
- pandas
- sqlite3
- flask
- flask_restx
- google.generativeai

Then you will need to create a .env file in the root directory of this repo to add a Gemini API key. Add the following to your .env file:
`GOOGLE_API_KEY=<your-api-key>`

You can create an API key for free in Google AI Studio [here](https://aistudio.google.com/).

Once the .env file is created, you can run the following in your terminal environment
`python3 z5360925.py`

This will start a development server in debug mode. You should then be able to access the API docs at the localhost URL running on port 5000. No path needed, the entire Swagger docs are accessible from the API at the root directory.

## API routes

The following routes can be used to query from the API.
- Create and edit stops
- Get info about a stop
- Edit a stop
- Delete a stop
- Get operator profiles
- Get guide

## Acknowledgements

This project was designed to be an assignment for the UNSW course COMP9321. It places RESTful API Guidelines at the core of all operations. 
