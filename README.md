# Restful-Booker-API-Automation
Automated CRUD lifecycle test suite for a hotel booking API using Postman and JavaScript
[Readme.md](https://github.com/user-attachments/files/25640772/Readme.md)
🚀 RESTful-Booker: End-to-End API Automation Suite
By Artashes Manoyan
📌 Project Overview
This project demonstrates a full CRUD (Create, Read, Update, Delete) lifecycle for a hotel booking system using the RESTful-Booker API. The goal was to build a robust, automated test suite in Postman that handles dynamic data synchronization and security authentication.

🛠️ Key Technical Features
Dynamic Data Hand-off: Successfully automated the extraction of bookingid and token from response bodies to be reused in subsequent requests.

Environment Management: Utilized Postman Environment variables to separate the Base URL from the test data, ensuring the collection is portable and scalable.

Auth Implementation: Integrated a secure token-based authentication flow for PUT and DELETE methods using Cookie headers.

Status Code Validation: Verified various server responses, including handling the unique "201 Created" quirk during deletion to confirm record removal via negative testing.

🧪 Test Scenarios Included
Create Booking (POST): Validates that a new reservation can be added and the ID is saved for future steps.

Auth Token Generation (POST): Requests a security key to unlock administrative permissions.

Get Details (GET): Confirms the server returns the correct user data for the specific ID created.

Update Booking (PUT): Modifies record details (e.g., changing first name to "QA Journey") and verifies the persistence of the change.

Delete & Verify (DELETE/GET): Removes the booking and performs a follow-up GET request to confirm a 404 Not Found response.

🚀 How to Run
Clone this repository.

Import the collection.json and environment.json files into Postman.

Select the "Testing 2026" environment.

Run the collection in order to see the full automated flow.
