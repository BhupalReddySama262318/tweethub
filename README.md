# TweetHub - A Django-based Social Media Platform

A Twitter-like social media platform built with Django that allows users to share posts with text and images.

## Features

- User Authentication (Register, Login, Logout)
- Create, Edit, and Delete Tweets
- Image Upload Support
- Responsive Design with Bootstrap
- Dark Theme Interface

## Live Demo

Visit the live demo at: [https://tweethub-ki95.onrender.com](https://tweethub-ki95.onrender.com)

Test Account:
- Username: `demo_user`
- Password: `demo123456`

Note: The demo is hosted on Render's free tier, so initial load might take a few seconds if the service is in sleep mode.

## Technologies Used

- Django 5.1.5
- Python
- Bootstrap 5
- SQLite3
- Gunicorn (for deployment)
- Pillow (for image processing)

## Prerequisites

- Python 3.x
- pip (Python package manager)

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd tweethub
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Apply database migrations:
   ```bash
   python manage.py migrate
   ```

5. Create a superuser (admin):
   ```bash
   python manage.py createsuperuser
   ```

6. Run the development server:
   ```bash
   python manage.py runserver
   ```

Visit `http://127.0.0.1:8000` in your browser to see the application.

## Project Structure

- `tweet/` - Main application directory containing views, models, and forms
- `twitter/` - Project configuration directory
- `templates/` - HTML templates
- `media/` - User uploaded files
- `static/` - Static files (CSS, JavaScript, Images)

## Features in Detail

### User Management
- User registration with email
- Login/Logout functionality
- Authentication required for creating/editing tweets

### Tweet Management
- Create new tweets with text and optional images
- Edit existing tweets
- Delete tweets
- View all tweets in a responsive grid layout

### Security Features
- CSRF protection
- User authentication
- Secure image upload handling

## Deployment

The project is configured for deployment on Render.com. Key deployment files:

- Procfile for Gunicorn configuration
- Requirements.txt for dependencies
- Static files configuration in settings.py

## Environment Variables

The following environment variables should be set in production:

- `SECRET_KEY` - Django secret key
- `DEBUG` - Set to False in production
- `ALLOWED_HOSTS` - List of allowed hosts

## Contributing

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Django Documentation
- Bootstrap Documentation
- Python Community
