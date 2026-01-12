# GreatKart

GreatKart is a fully featured e-commerce web application built using Django. It supports complete product management, user authentication, shopping cart functionality, and order processing.

## Features

- **Custom User Authentication**: 
  - Login with Email instead of Username.
  - Dashboard for tailored user experience.
- **Product Management**:
  - Full product catalog with categories.
  - Product variations (finding products by specific colors or sizes).
- **Shopping Cart**:
  - Add/Remove items.
  - Increment/Decrement quantities.
  - Guest cart support (session-based).
- **Search**: 
  - Keyword search for products.
- **Admin Panel**: 
  - Customized Django admin for managing products, categories, and variations.

## Tech Stack

- **Backend**: Python, Django
- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap (Jinja2 Templates)
- **Database**: SQLite (Development)
- **Media**: Pillow for image handling

## Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd "04 Greatkart"
   ```

2. **Create and activate a virtual environment**
   ```bash
   # Windows
   python -m venv env
   .\env\Scripts\activate

   # Linux/Mac
   python3 -m venv env
   source env/bin/activate
   ```

3. **Install Dependencies**
   It is recommended to create a `requirements.txt` file or install manually:
   ```bash
   pip install django pillow
   ```

4. **Apply Migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create a Superuser (Admin)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the Server**
   ```bash
   python manage.py runserver
   ```

## Project Structure

- `accounts/`: Handles user registration, login, and custom user models.
- `store/`: Manages products, product details, and search logic.
- `carts/`: Handles cart logic, adding items, and cart sessions.
- `catagory/`: Manages product categories.
- `greatkart/`: Main project configuration structure (`settings.py`, `urls.py`).
- `templates/`: HTML templates for the frontend.
- `static/`: Static files (CSS, JS, Images).
- `media/`: User-uploaded media (Product images).

## Contributing

1. Fork the project.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.
