# Onboarding API Documentation
This document provides an overview of the endpoints and models available in the Onboarding API. The API is designed to manage student information within the context of STD22019.

## Table of Contents

- [Introduction](#introduction)
- [Endpoints](#endpoints)
  - [Get All Students](#get-all-students)
  - [Add Student](#add-student)
- [Data Models](#data-models)
  - [StudentsResponse](#studentsresponse)
  - [AddStudentsResponse](#addstudentsresponse)
  - [StudentInput](#studentinput)

## Endpoints

### Get All Students

- **URL**: `/students`
- **Method**: GET
- **Description**: Retrieve a list of all students.
- **Response**:
  - Successful Response (200 OK): Returns a list of students.
  - Internal Server Error (500): Indicates a server error.

### Add Student

- **URL**: `/student`
- **Method**: POST
- **Description**: Add a new student to the system.
- **Request Body**: Requires a JSON object representing the new student.
- **Response**:
  - Successful Response (200 OK): Returns the newly added student information.
  - Internal Server Error (500): Indicates a server error.

## Data Models

### StudentsResponse

Represents a response containing student information.

- `id` (string): Student ID.
- `name` (string): Student name.
- `birthDate` (string, date format): Student birth date.

### AddStudentsResponse

Represents a response containing newly added student information.

- `id` (string): Student ID.
- `name` (string): Student name.
- `birthDate` (string, date format): Student birth date.

### StudentInput

Represents the input data for adding a new student.

- `id` (string): Student ID.
- `name` (string): Student name.
- `birthDate` (string, date format): Student birth date.

## Contact

For any questions or concerns regarding this API, please contact at [hei.fifaliana@gmail.com](mailto:hei.fifaliana@gmail.com).