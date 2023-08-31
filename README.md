# PyTacos
🌮 Oliver: Your Friendly Mexican Restaurant Order Assistant 🌮  Introducing Oliver, the charming chatbot that takes your order in a Mexican restaurant with a personalized touch! Say adios to traditional menus and hola to a new, interactive way of placing your favorite Mexican dishes.

# Oliver Chatbot Project

Welcome to the Oliver Chatbot project! This project features a conversational chatbot designed to assist users in choosing delicious Mexican dishes. The chatbot interacts with users through a user-friendly HTML interface and utilizes Google Dialogflow for natural language processing.

## Table of Contents

- Introduction
- Setup
  - Database Setup
  - Backend Installation
  - Dialogflow Configuration
- Usage

## Introduction

Oliver is a conversational chatbot that helps users explore and select tasty Mexican dishes. It combines Google Dialogflow for natural language understanding and a FastAPI backend for connecting to the project's database.

## Setup

Follow these steps to set up and run the project locally.

### Database Setup 

1. Navigate to the `database` folder.
2. Open the SQL file and execute the queries in your database management tool.
3. Make sure to replace variables in the queries with your actual database elements.

### Backend Installation

1. Install required Python libraries for the backend:

   ```bash
   pip install -r backend/requirements.txt

2. Start the FastApi Server:

   ```bash
   uvicorn backend.main:app --host 0.0.0.0 --port port_number

### Dialogflow Configuration
1. Import the Dialogflow agent included in the oliver-chatbot folder.
2. To connect the agent to the database, run the FastAPI server as mentioned above.
3. Navigate to the ngrok app in the backend folder in your terminal.
4. Run the following command to create a secure URL:

ngrok http port_number

5. Take note of the secure URL provided by ngrok.
6. In the Dialogflow agent settings, go to the Fulfillment tab.
7. Set the secure ngrok URL as the webhook URL.
8. The chatbot will function as long as the ngrok URL is active.

### Usage 

1. Open the HTML file to access the chatbot interface.
2. Interact with the chatbot to explore and choose Mexican dishes.
3. Enjoy a virtual culinary experience with Oliver!
