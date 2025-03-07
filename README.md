# Email Verification in Django

This project is a simple Django-based user registration system with email verification.

## Features
- User registration with email and password
- Email verification using a one-time code
- Authentication and login after successful verification

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/email-verification-django.git
   cd email-verification-django
   ```

2. Create a virtual environment and activate it:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

4. Configure your email settings in `settings.py`:
   ```python
   EMAIL_BACKEND = "django.core.mail.backends.smtp.EmailBackend"
   EMAIL_HOST = "smtp.gmail.com"
   EMAIL_PORT = 587
   EMAIL_USE_TLS = True
   EMAIL_HOST_USER = "your-email@gmail.com"
   EMAIL_HOST_PASSWORD = "your-email-password"
   ```

5. Run migrations:
   ```sh
   python manage.py migrate
   ```

6. Start the development server:
   ```sh
   python manage.py runserver
   ```

## Usage
- Open `http://127.0.0.1:8000/register/` in your browser.
- Enter your email and password.
- Check your email for the verification code.
- Enter the verification code to complete registration.
