# Disney Bot - GenAI

A Disney Gen AI bot specializing in restaurant reservations that interacts with users through Vertex AI to manage their dining plans. Through the uploaded files, the bot can take in key parameters such as party size, desired time, and restaurant location to reference a Cloud Firestore database.

## Webhooks
- changeReservation: Modifies an existing dining reservation by including the restaurant, time, and party size, ensuring that the user's new preferences are accurately reflected in the database.

- checkAvailability: Triggered when a user inquiries about the availability of a dining reservation at a specific restaurant for a time and party size. Database checks for current availability status and provides options if reservation slot has been booked.

- displayReservation: A webhook that confirms the details of a user's dining reservation. It displays the reservation information including restaurant name, time, and party size to the user and saves the information to the database.

- getNumber: Authenticates a user's phone number to an existing Disney Account by referencing Cloud Firestore DB.

##  Language
- Node.JS

## Dependencies
- "actions-on-google": "^2.5.0",
- "firebase-admin": "^8.2.0",
- "firebase-functions": "^2.0.2",
- "dialogflow": "^0.6.0",
- "dialogflow-fulfillment": "^0.6.1"
