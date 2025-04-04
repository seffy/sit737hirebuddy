# HireBuddy (DRAFT)

HireBuddy is a cloud-native web application designed to connect users with friendly companions for casual social activities such as meals, shopping, outdoor fun, family gatherings, or simply having a chat. The core features will include posting companionship requests, browsing listings, viewing profiles, and accepting invitations.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Architecture](#architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Future Enhancements](#future-enhancements)
- [Troubleshooting](#troubleshooting)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction
HireBuddy aims to provide a friendly platform for people looking to connect with like-minded individuals for various social engagements..........

## Features
- **User Authentication:** Secure registration and login using bcrypt for password hashing.
- **Dynamic Content Rendering:** Server-side dynamic rendering with EJS templates.
- **MVC Architecture:** A clear separation between Models, Views, and Controllers for maintainability.
- **Scalable Design:** Optimized for deployment on cloud platforms like Google Cloud Platform (GCP).
- **Responsive UI:** Simple and clean design ensuring accessibility across devices.

## Architecture
HireBuddy follows the Model-View-Controller (MVC) design pattern:
- **Model:** Defined using MongoDB schemas (e.g., the User model) to manage data.
- **View:** EJS templates render dynamic HTML pages with embedded JavaScript.
- **Controller:** Express controllers handle business logic, process requests, and interact with the database.
- **Routes:** Express routes map HTTP requests to their corresponding controller functions.
- TBD


## Installation

### Prerequisites
- [Node.js](https://nodejs.org/) (v12 or above)
- [npm](https://www.npmjs.com/)
- [MongoDB](https://www.mongodb.com/) (local installation or cloud instance)
- [Docker](https://www.docker.com/) for containerized deployment
- TBD

### Setup Steps
1. **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/sit737hirebuddy.git
    cd sit737hirebuddy
    ```

2. **Install Dependencies:**
    ```bash
    npm install
    ```
    This command installs required packages such as `express`, `mongoose`, `ejs`, `body-parser`, and `bcrypt`.

3. **Configure MongoDB Connection:**
   Ensure that your MongoDB instance is running. You may need to update the connection string in `server.js`:
    ```javascript
    mongoose.connect('mongodb://localhost/hirebuddy', { useNewUrlParser: true, useUnifiedTopology: true });
    ```

4. **Docker Setup:**

## Usage

### Running the Application
To start the HireBuddy application, run:

    node server.js

## Project Structure 

	HireBuddy/
	├── controllers/
	│   └── authController.js    # Handles authentication logic
	├── models/
	│   └── User.js              # Defines the User schema for MongoDB
	├── routes/
	│   └── authRoutes.js        # Maps URLs to controller functions
	├── views/
	│   ├── login.ejs            # Template for the login page
	│   └── register.ejs         # Template for the registration page
	├── public/
	│   ├── css/
	│   │   └── style.css        # Styling for the application
	│   └── js/
	│       └── script.js        # Client-side JavaScript
	└── server.js                # Entry point for the application

## Technologies Used
## Future Enhancements
## Troubleshooting
## License
## Author
	JJS
## Acknowledgements
	- Developed as part of the SIT737 Cloud Native Application Development unit at Deakin University.
