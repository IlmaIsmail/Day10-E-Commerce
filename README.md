# Error Handling in Employee Management System

## Department Management Service
A Spring Boot REST API service for managing department information with comprehensive error handling and JPA integration.

## Overview
This service provides CRUD operations for department management with built-in exception handling and data validation. It's designed for educational institutions or organizations that need to manage departmental information and employee associations.

## Architecture
The application follows a layered architecture pattern:

Model Layer: JPA entities with proper relationships
Repository Layer: Spring Data JPA repositories
Service Layer: Business logic implementation
Exception Handler: Centralized error handling

## Features
1. Department CRUD Operations
2. Data Validation
3. Proper HTTP status codes

## API Endpoints
   Get All Departments

![Screenshot (83)](https://github.com/user-attachments/assets/1c3d5b01-51bb-44aa-a235-a6ff696150df)

   Get Department by ID

![Screenshot (84)](https://github.com/user-attachments/assets/8da4464c-21b4-4fb7-a377-0baa6469fa9c)

   Error Response (404):

![Screenshot (2)](https://github.com/user-attachments/assets/63225aae-ef48-49bc-a6db-9746183d00a2)

   Add New Department

![Screenshot (3)](https://github.com/user-attachments/assets/5beda790-77b7-4f11-aa33-b014662d2a99)

   Error Response (400) - Duplicate ID:

![Screenshot (4)](https://github.com/user-attachments/assets/c64502d7-234f-4be7-9f6c-4f31d406f07e)


## Exception Handling
The service implements comprehensive exception handling:

 
      EntityNotFoundException	- 404	- Department not found
      DuplicateKeyException	- 400 - Duplicate department ID
      Exception	            - 500 - Generic server errors

   

