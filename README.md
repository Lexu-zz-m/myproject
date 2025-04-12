# RFM PrintShop: E-Commerce Platform for Custom Printing Services - Django Project

A secure and user-friendly Django-based e-commerce web application built for a local custom printing shop. This platform allows customers to browse services, upload design files, place orders, and manage transactions online. It features a full authentication system including user registration, login, logout, and a personalized dashboard for tracking order history and status.

##  Features

- User Registration & Login (with session management)
- Secure password handling using Django's built-in auth system
- User Dashboard with:
  - Personalized greeting and user info display
  - Recent orders summary
  - Navigation to shop and other sections
- Responsive Order Interface styled with modern CSS
- Custom Order Forms with file upload support (for printing materials)
- Email-based Login System (with password visibility toggle)
- Logout Functionality accessible from the user panel
- Dynamic Messaging for errors and notifications
- Navigation Panel with icons for quick access (Home, Orders, Gallery, Profile)
- Clean and Responsive UI built with HTML5 & CSS3, mobile-friendly

## User Authentication System

# Registration
- Users can create an account through the /register/ route.
- The sign-up form includes:
    - Full Name
    - Email Address (must be unique)
    - Password + Confirmation (with toggle visibility option)
- Custom-styled form using modern, responsive CSS.
- Backend uses Django’s UserCreationForm extended to support additional fields.

# Login
- Users can log in at /login/.
- Styled login interface with:
    - Email and password fields
    - “Remember me” checkbox
    - Password visibility toggle
    - Forgot password link
- Credentials are authenticated using Django’s AuthenticationForm.
- Upon successful login, users are redirected to their personalized dashboard.

# Dashboard
- After login, users are taken to their dashboard at /dashboard/ or /home/.
- Displays:
    - Welcome message using user's name
    - Order status and recent order history
    - Navigation to shop or place new orders
- Responsive layout and personalized user data using {{ user.first_name }} and {{ user.email }}.

##  Setup Instructions

```bash
# Clone the repository
git clone https://github.com/MarcKyle/moni-project.git
cd myproject

# Install dependencies
pip install -r requirements.txt

# Apply migrations
python manage.py migrate

# Start the development server
python manage.py runserver
```

