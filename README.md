![image](https://github.com/user-attachments/assets/50cc810a-953d-4530-b981-5a7a367e6b7d)


# Simple Notes RESTful API

This project is my first experience building a RESTful API as part of my learning journey in the IDCamp 2024 training program, focusing on the backend development track. I am enrolled in the "Belajar Backend Pemula dengan Javascript" class created by Dicoding Indonesia.

## About This Project

I built a simple RESTful API for a notes application, which allows users to perform CRUD operations:

- **Create** - Add new notes to the application.
- **Read** - View existing notes.
- **Update** - Modify notes as needed.
- **Delete** - Remove notes from the application.

These core functionalities are collectively referred to as **CRUD** operations.

For the front-end (client) side, a web application has already been created and deployed. You can access it via the following link: [Notes App Web](http://notesapp-v1.dicodingacademy.com/).

This project also involves deployment using AWS EC2, where I deployed the backend API. I used **PM2** to manage the application processes in a production environment.

### Technology Stack

- **Back-End Framework**: Hapi.js (Node.js)
- **Linting Tool**: ESLint
- **Deployment**: AWS EC2
  ![image](https://github.com/user-attachments/assets/930815b1-8e38-4331-b827-b9a7458c5974)

- **Process Manager**: PM2 (for managing the app in production)


## API Endpoints

- **POST** `/notes` - Create a new note
- **GET** `/notes` - Retrieve all notes
- **GET** `/notes/{id}` - Retrieve a specific note
- **PUT** `/notes/{id}` - Update a specific note
- **DELETE** `/notes/{id}` - Delete a specific note

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/emhafis/notes-app-back-end.git

2. Navigate to the project directory:
   ```bash
   cd simple-notes-api

4. Install dependencies:
   ```bash
   npm install

6. Run the application:
   ```bash
   npm start

## Deployment

1. Launch an EC2 instance and SSH into it.
   ```bash
   git clone https://github.com/emhafis/notes-app-back-end.git

2. Clone the repository to the instance:
   ```bash

   
3. Navigate to the project directory:
   ```bash
   cd notes-app-back-end
   
4. Install dependencies:
   ```bash
   npm install
   
5. Install PM2 globally:
   ```bash
   sudo npm install pm2 -g
   
6. Start the application using PM2:
   ```bash
   pm2 start npm --name "notes-api" -- run "start:prod"
    
7. Ensure that PM2 is set to start on boot:
   ```bash
   pm2 startup
   pm2 save
