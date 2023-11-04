# htr23 API

**htr23** is a simple Kotlin API that allows you to perform CRUD (Create, Read, Update, Delete) operations on Users, Activities, and BMI records. It provides endpoints for managing these entities. This README provides an overview of the API and how to use it.

## Table of Contents

- [API Endpoints](#api-endpoints)
- [Authentication](#authentication)
- [Entities](#entities)
- [Usage](#usage)
- [swagger](../swagger/htr23-activity.yaml)


## API Endpoints

### Users

- **GET /api/users**: Get a list of all users.
- **POST /api/users**: Create a new user.
- **GET /api/users/{user-id}**: Get a specific user by ID.
- **PATCH /api/users/{user-id}**: Update an existing user.
- **DELETE /api/users/{user-id}**: Delete a user by ID.

#### User Activities

- **GET /api/users/{user-id}/activities**: Get a list of activities for a specific user.
- **DELETE /api/users/{user-id}/activities**: Delete all activities for a specific user.

#### User BMI Records

- **GET /api/users/{user-id}/bmis**: Get a list of BMI records for a specific user.
- **DELETE /api/users/{user-id}/bmis**: Delete all BMI records for a specific user.

- **GET /api/users/email/{email}**: Get a user by email.

### Activities

- **GET /api/activities**: Get a list of all activities.
- **POST /api/activities**: Create a new activity.
- **GET /api/activities/{activity-id}**: Get a specific activity by ID.
- **PATCH /api/activities/{activity-id}**: Update an existing activity.
- **DELETE /api/activities/{activity-id}**: Delete an activity by ID.

### BMI Records

- **GET /api/bmis**: Get a list of all BMI records.
- **POST /api/bmis**: Create a new BMI record.
- **GET /api/bmis/{bmi-id}**: Get a specific BMI record by ID.
- **PATCH /api/bmis/{bmi-id}**: Update an existing BMI record.
- **DELETE /api/bmis/{bmi-id}**: Delete a BMI record by ID.

## Authentication

This API does not currently require authentication yet. But following iterations will.

## Entities

The API works with the following entities:

- **User**: Represents a user with attributes "name" and "email."
- **Activity**: Represents an activity with attributes "id," "description," "duration," "calories," "started," and "userId."
- **BMI Record**: Represents a BMI (Body Mass Index) record with attributes "id," "age," "height," "weight," and "userId."

## Usage

1. Clone the repository: `git clone https://github.com/bopojoe/htr23.git`
2. Build and run the API using intellij.
3. Access the API using your preferred HTTP client (e.g., Postman or cURL) or integrate it into your applications.



 
