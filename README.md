# VChat

VChat is a real-time chat application designed during our training period at Vcube Software Solutions. The primary purpose of this application is to enhance communication and coordination between students and coordinators in our institute to improve academic standards.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Security](#security)
- [Contributors](#contributors)

## Features

- Real-time messaging between students and coordinators.
- Creation of chat rooms for different topics or groups.
- Secure user authentication and authorization.
- User-friendly and dynamic interface using HTML, CSS, and Bootstrap.
- Real-time updates with WebSockets and Redis Channels.
- Coordinator-only authorization to add and confirm student details.
- Data storage using SQLite database.

## Technologies Used

### Backend

- **Django Framework**: For handling HTTP requests, database interactions, and serving web pages.
- **Python**: For backend logic and processing.
- **Django Channels**: For real-time WebSocket connections and asynchronous communication.
- **Redis**: For message brokering and handling real-time events.

### Frontend

- **HTML5**: For structuring the web pages.
- **CSS3**: For styling the application.
- **JavaScript**: For interactive and dynamic features.

### Database

- **SQLite**: For storing user data, messages, and chat room information.

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your_username/vchat.git
    cd vchat
    ```

2. **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Apply migrations:**
    ```bash
    python manage.py migrate
    ```

5. **Run the Redis server:**
    Make sure Redis is installed and running on your machine. Refer to the [Redis documentation](https://redis.io/documentation) for installation instructions.

6. **Run the development server:**
    ```bash
    python manage.py runserver
    ```

7. **Access the application:**
    Open your web browser and go to `http://127.0.0.1:8000/`

## Usage

- **Register and Login:**
    Users can register and log in to the application securely.
- **Create or Join Chat Rooms:**
    Users can create new chat rooms or join existing ones to participate in discussions.
- **Real-Time Messaging:**
    Messages sent in a chat room are delivered in real-time to all participants.
- **Private Messaging:**
    Users can send private messages to each other.
- **Coordinator Actions:**
    Coordinators can add and confirm student details to ensure only enrolled students can access the chat application.

## Security

- **Authentication and Authorization:**
    The application uses secure authentication and authorization processes to protect user data and restrict access to authorized users only.
- **Data Protection:**
    Only coordinators have the authorization to add and confirm student details, ensuring that only enrolled students can use the application.

## Contributors

This project was developed by a group of trainees at Vcube Software Solutions.


