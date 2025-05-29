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


   Get Department by ID


   Error Response (404):


   Add New Department


   Error Response (400) - Duplicate ID:


## Exception Handling
The service implements comprehensive exception handling:

 
EntityNotFoundException	- 404	- Department not found
DuplicateKeyException	- 400 - Duplicate department ID
Exception	            - 500 - Generic server errors

   
