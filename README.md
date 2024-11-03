# Simple Notes RESTful API

This project is my first experience building a RESTful API as part of my learning journey in the IDCamp 2024 training program, focusing on the backend development track. I am enrolled in the "Belajar Backend Pemula dengan Javascript" class created by Dicoding Indonesia.

## About This Project

I built a simple RESTful API for a notes application, which allows users to perform CRUD operations: 

- **Create** - Add new notes to the application.
- **Read** - View existing notes.
- **Update** - Modify notes as needed.
- **Delete** - Remove notes from the application.

This functionality is commonly referred to as CRUD operations. 

For the front-end (client) side, a web application has already been created and deployed. You can access it via the following link: [Notes App Web](http://notesapp-v1.dicodingacademy.com/).

### Technology Stack

- **Back-End Framework**: Hapi.js (Node.js)
- **Linting Tool**: ESLint

## API Endpoints

- **POST** `/notes` - Create a new note
- **GET** `/notes` - Retrieve all notes
- **GET** `/notes/{id}` - Retrieve a specific note
- **PUT** `/notes/{id}` - Update a specific note
- **DELETE** `/notes/{id}` - Delete a specific note

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/emhafis/simple-notes-api.git

2. Navigate to the project directory:
   ```bash
   cd simple-notes-api

4. Install dependencies:
   ```bash
   npm install

6. Run the application:
   ```bash
   npm start
