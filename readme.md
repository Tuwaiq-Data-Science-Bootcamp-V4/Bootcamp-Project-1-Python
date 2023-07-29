# Event Ticket Booking System

This is a simple Event Ticket Booking System implemented in Python. The system allows users to browse available events, search for specific events, add tickets to their shopping cart, remove tickets from the cart, modify ticket quantities, and proceed to checkout. Additionally, it provides user recommendations based on their purchase history and event tags.

## Features

- Browse Events: Users can view a list of all available events along with their basic information such as event name, summary, time, price, and place.

- Search for an Event: Users can search for events by providing a keyword, and the system will display a list of events whose names match the keyword.

- Add Tickets to the Shopping Cart: Users can add tickets to their shopping cart by specifying their user ID, the Event ID, and the desired quantity of tickets.

- Remove Tickets from the Shopping Cart: Users can remove tickets from their shopping cart by providing their user ID and the Event ID.

- Modify Ticket Quantity: Users can modify the number of tickets in their shopping cart by providing their user ID, the Event ID, and the new quantity.

- Checkout: Users can proceed to checkout, where they can view their shopping cart items, the total cost, and then confirm the payment.

- Get User Recommendations: Users can get event recommendations based on their purchase history and the tags associated with the events they have previously purchased.

## Usage

1. Install Python: Make sure you have Python installed on your system. You can download it from the official website (https://www.python.org/) and follow the installation instructions.

2. Run the Application: Save the provided Python code in a file, e.g., `event_booking_system.py`, and run the script using the Python interpreter.

3. Interact with the Application: The application will display a main menu with different options. You can choose an option by entering the corresponding number (1-8). Follow the prompts to perform various actions, such as browsing events, adding tickets to the cart, searching for events, etc.

4. Event and User Data: The code includes sample event data (two events) and sample user data (one user). You can add more events and users by modifying the code accordingly or load event and user data from files or a database.

5. Data Persistence (Optional): The code includes optional code to save the `events` list and `users` dictionary to files (`events.json` and `users.json`) for data persistence. If you want to enable data persistence, make sure to uncomment the relevant lines.

## Note

This is a basic implementation of an event ticket booking system for learning purposes. In a real-world scenario, a complete system would require additional features such as user authentication, secure payment processing, error handling, and data validation. Additionally, you may consider using a database to store event and user data for scalability and reliability.
