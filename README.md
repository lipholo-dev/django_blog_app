Django Blog App
A simple yet functional blog application built with Django that allows users to create and share blog posts. This blog platform provides a clean interface for reading posts and an admin 
panel for content management.
Table of Contents

Features
Technologies Used
Installation
Usage
Project Structure
Credits

Features
Display blog posts in reverse chronological order
Detailed view for individual blog posts
Admin panel for content management
Custom signature for blog posts
Responsive design

Technologies Used
Python
Django
HTML/CSS
Bootstrap 5.3.3
SQLite database
Django Admin

Installation
Follow these steps to set up the project locally:
bash# Clone the repository
git clone git@github.com:lipholo-dev/django_blog_app.git

# Navigate to the project directory
cd django_blog_app

# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Apply migrations
python manage.py migrate

# Create a superuser
python manage.py createsuperuser

# Run the development server
python manage.py runserver
Usage
After installation, you can access the blog at http://127.0.0.1:8000/blog/.

Admin Access
Go to http://127.0.0.1:8000/admin/
Log in with your superuser credentials
From here you can add, edit, and delete blog posts

Adding a Blog Post
Log in to the admin panel
Click on "Posts" in the admin dashboard
Click "Add Post" in the top right corner
Fill in the title, body, signature, and date
Click "Save" to publish your blog post

Viewing Blog Posts
Visit http://127.0.0.1:8000/blog/ to see a list of all blog posts
Click on a post title to view the full post at http://127.0.0.1:8000/blog/<post_id>/


Project Structure
blog_app/
│
├── blog/                  # Blog application
│   ├── __pycache__/       # Python cache files
│   ├── migrations/        # Database migrations
│   │   ├── __pycache__/   
│   │   └── 0001_initial.py
│   ├── templates/         # HTML templates
│   │   ├── blog.html      # Template for blog list view
│   │   ├── header.html    # Header template
│   │   └── post.html      # Template for individual post view
│   ├── __init__.py
│   ├── admin.py           # Admin configuration
│   ├── apps.py
│   ├── models.py          # Database models with Post class
│   ├── tests.py
│   ├── urls.py            # URL routing for blog app
│   └── views.py           # View functions (uses generic views)
│
├── mySite/                # Project settings directory
│   ├── __pycache__/       
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py        # Django settings
│   ├── urls.py            # Main URL routing
│   └── wsgi.py            # WSGI configuration
│
├── personal/              # Additional application
│   ├── __pycache__/
│   ├── migrations/
│   ├── templates/
│   │   ├── about.html
│   │   ├── index.html
│   │   └── store.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
│
├── db.sqlite3             # SQLite database file
├── manage.py              # Django management script
└── README.md              # This file

Credits
Developed by Hlomelang Lipholo (lipholo-dev)
Created as part of the HyperionDev Full Stack Developer course
