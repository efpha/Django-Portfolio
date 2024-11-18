# **Portfolio Website**
A Django-based portfolio website. The site includes a contact form that allows visitors to leave messages, which are stored in a database for easy access.
---

## **Features**
- Fully responsive design using **Bootstrap 5**.
- Separate pages for:
  - Home
  - About
  - Projects
  - Contact
- Contact form with validation for:
  - Name
  - Email
  - Phone
  - Message (minimum 100 characters).
- Stores messages in a Django database.
- Provides feedback to users upon successful form submission.

---

## **Setup Instructions**
### **1. Set Up Virtual Environment**
Create and activate a virtual environment:
```bash
python -m venv myenv
myenv\Scripts\activate     
```

### **2. Install Dependencies**
Run the following command to install the required dependencies:
```bash
pip install django
```

### **Installed Dependencies**
- `Django==5.1.3`: The web framework used to build the portfolio website.
- **Bootstrap 5** (via CDN): Used for responsive design and styling. It’s included in the HTML through a CDN in the `base.html` file.
- `sqlite3`: The default database used by Django for development.

### **3. Configure the Database**
The project uses SQLite by default.

Run the migrations to set up the database:
```bash
python manage.py makemigrations
python manage.py migrate
```

### **4. Run the Development Server**
Start the server:
```bash
python manage.py runserver
```

Access the website at `http://127.0.0.1:8000/`.

---

## **Additional Notes**

- **Bootstrap**: The project uses **Bootstrap 5** for responsive design and layout. It’s linked via a CDN in the `base.html` template.
- **Static Files**: To ensure that the static files are correctly set up in `settings.py`.
- **Admin Panel**: Manage contact form submissions and other admin tasks by creating a superuser:
  ```bash
  python manage.py createsuperuser
  ```
  Then access the admin panel at `/admin/`.


