# Lunchly Web App

Lunchly is a web application for managing customer reservations at a restaurant. It allows users to view a list of customers, search for customers by name, add new customers, view customer details, edit customer information, and add reservations for customers.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Routes](#routes)
  - [Homepage](#homepage)
  - [Search](#search)
  - [Add New Customer](#add-new-customer)
  - [View Customer Details](#view-customer-details)
  - [Edit Customer](#edit-customer)
  - [Add Reservation](#add-reservation)

## Installation

To run Lunchly locally, follow these steps:

1. Clone the repository: `git clone <repository-url>`
2. Navigate to the project directory: `cd lunchly`
3. Install dependencies: `npm install`
4. Start the server: `npm start`
5. Open your browser and go to `http://localhost:3000`

## Usage

Once the server is running, you can use Lunchly to manage customer reservations. Navigate through the different routes to perform actions such as adding new customers, editing customer details, and adding reservations.

## Routes

### Homepage

- Route: `/`
- Method: GET
- Description: Displays a list of all customers.

### Search

- Route: `/search/`
- Method: GET
- Description: Allows searching for customers by name.
- Query Parameters:
  - `name`: The name to search for.

### Add New Customer

- Route: `/add/`
- Method: GET
- Description: Displays a form for adding a new customer.
- Method: POST
- Description: Handles adding a new customer.
- Form Fields:
  - `firstName`: First name of the customer.
  - `lastName`: Last name of the customer.
  - `phone`: Phone number of the customer.
  - `notes`: Additional notes about the customer.

### View Customer Details

- Route: `/:id/`
- Method: GET
- Description: Displays details of a specific customer, including reservations.

### Edit Customer

- Route: `/:id/edit/`
- Method: GET
- Description: Displays a form for editing customer details.
- Method: POST
- Description: Handles updating customer information.
- Form Fields:
  - `firstName`: Updated first name of the customer.
  - `lastName`: Updated last name of the customer.
  - `phone`: Updated phone number of the customer.
  - `notes`: Updated notes about the customer.

### Add Reservation

- Route: `/:id/add-reservation/`
- Method: POST
- Description: Handles adding a new reservation for a customer.
- Form Fields:
  - `startAt`: Start date and time of the reservation.
  - `numGuests`: Number of guests for the reservation.
  - `notes`: Additional notes about the reservation.

### Made By: Samie Smilz
