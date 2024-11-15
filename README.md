Real-Time Chat Application
Welcome to Jomapp, a real-time chat application built with Django, Django Channels, and WebSockets. This project enables users to join chat rooms and communicate with each other in real-time. The application uses WebSockets for efficient, real-time message exchange, and supports basic functionalities like room creation, message sending, and authentication.

Features
Real-time chat functionality using WebSockets and Django Channels.
Create and join multiple chat rooms.
Message history is displayed for each chat room.
User authentication to send messages.
Responsive design to support various screen sizes and devices.
Real-time notifications for incoming messages.
Tech Stack
Backend: Django, Django Channels
Frontend: HTML, CSS (Bootstrap for responsiveness)
Real-time Communication: WebSockets
Database: SQLite (default in Django, can be configured to use other databases)
Channel Layer: Redis (for message brokering)
Deployment: (Specify how you plan to deploy your app, e.g., Heroku, Docker, etc.)
Installation
Clone the repository
First, clone the project repository to your local machine:

bash
Copy code
git clone https://github.com/Jomwanje/jomapp.git
Set up a virtual environment
It's recommended to use a virtual environment to manage your project's dependencies:

bash
Copy code
cd jomapp
python -m venv .venv
source .venv/bin/activate  # On Windows, use .venv\Scripts\activate
Install dependencies
Install the required dependencies listed in requirements.txt:

bash
Copy code
pip install -r requirements.txt
Install Redis
Since the project uses Django Channels with Redis for real-time message delivery, you will need to install Redis:

Install Redis on your local machine:

Download and install Redis for your system.
Alternatively, you can use Docker to run Redis.
Start Redis server (if using Redis locally):

bash
Copy code
redis-server
Database Migrations
Run the following commands to apply the necessary migrations for the database:

bash
Copy code
python manage.py migrate
Create a superuser (optional)
If you need an admin user to manage the application, run:

bash
Copy code
python manage.py createsuperuser
Run the Development Server
Finally, run the development server to see the application in action:

bash
Copy code
python manage.py runserver
Visit http://127.0.0.1:8000 in your web browser to access the app.
