📌 Project Overview

This repository contains the server-side (backend) code for a dating application that I built. The backend is implemented as a RESTful API and is responsible for authentication, user management, matching logic, messaging, and secure data access.

The goal of this project was to gain hands-on experience building a real-world backend using modern best practices, clean architecture, and industry-standard tools.

🛠️ Tech Stack

ASP.NET Core Web API

C#

Entity Framework Core

SQL Server / SQLite

JWT Authentication

AutoMapper

Cloudinary (image hosting)

Swagger / OpenAPI

🧱 Architecture

I structured the backend using a layered architecture to keep the code clean, maintainable, and scalable:

Controllers handle HTTP requests and responses

DTOs control the shape of data sent to and from the client

Entities represent domain models and database tables

Data Layer manages database access using Entity Framework Core

Helpers / Services contain shared business logic (token creation, pagination, photo handling)

Middleware handles global error handling and request processing

🔐 Authentication & Authorization

Implemented JWT-based authentication

Secured protected endpoints so only authenticated users can access them

Passwords are hashed and salted for security

Authorization ensures users can only modify or access their own data

👤 User Management

I implemented full user profile management, including:

User registration and login

Viewing and updating user profiles

Uploading, deleting, and setting a main profile photo

Filtering users by preferences (e.g. gender)

Pagination and sorting for user lists

💘 Dating App Functionality (Backend)

The API supports core dating app features such as:

Like and dislike functionality

Match detection when likes are mutual

Messaging between matched users

Message threads with read/unread status

Secure validation to prevent unauthorized interactions

🗄️ Database & Data Persistence

Used Entity Framework Core with a code-first approach

Created and managed database migrations

Defined relationships between users, photos, likes, and messages

Optimized queries using eager loading where appropriate

📸 Photo Management

Integrated Cloudinary for image storage

Photos are stored externally; only URLs are saved in the database

Implemented validation to ensure only the photo owner can modify or delete images

⚙️ API Features

RESTful endpoint design

Consistent response formats

Pagination metadata included in response headers

Centralized exception handling

API documentation and testing via Swagger

🎯 What I Learned

Through this project, I gained experience with:

Building a production-style REST API

Implementing secure authentication and authorization

Applying clean architecture and separation of concerns

Using DTOs to protect and shape data

Managing relational data efficiently

Writing scalable and maintainable backend code

🚀 Running the Project

Clone the repository

Configure appsettings.json (database connection and Cloudinary credentials)

Apply database migrations

Run the API using Visual Studio or dotnet run

Test endpoints using Swagger UI

📚 Acknowledgments

This project was built as part of a Udemy course by Neil Cummings and is intended for learning and portfolio demonstration purposes.
