# University Marketplace

*This project was developed as a 2nd-year computing project for the WAD2 (Web-App Development) course.*

## About the Project
University Marketplace is a secure web-based platform designed exclusively for students to buy and sell academic materials and lifestyle essentials within a verified campus network. 

The project aims to promote **Sustainability** by reducing waste and encouraging the reuse of goods, while offering **Savings** through affordable second-hand options for students. 

**Live Demo:** [University Marketplace on PythonAnywhere](https://5070850h.pythonanywhere.com/marketplace/)

## Key Features
* **Smart Discovery:** Advanced search functionality featuring live AJAX updates, query parameters, and filters by tag and price.
* **Trust-Based Profiles:** Individual seller pages display dynamically calculated average ratings based on buyer feedback.
* **Automated Transactions:** The system performs an automated balance check before confirming any sale, seamlessly processing payments.
* **Integrated Review System:** Upon purchase, buyers are redirected to a review page to leave ratings, which update the seller's reputation in real-time.
* **User Dashboards:** Dedicated profile pages split into distinct sections showing user information, items currently for sale, and a history of items bought.

## Application Design
* **Responsive UI:** Built with responsive Bootstrap columns to adapt to various screen sizes, maintaining a clean and minimal layout.
* **Product Cards:** Items are displayed in standardized cards showing the image, title, category, seller, and price at a glance.
* **Intuitive Navigation:** A consistent top navigation bar provides quick access to Home, Search, Profile/Sell, and Register/Login.
* **Streamlined Forms:** Pages for selling, editing, and deleting items utilize simple forms with clear labels and color-coded, consistently styled action buttons.

## Tech Stack
**Backend:** Python (3.11.14), Django (2.2.28), SQLite, Pillow (12.1.0)  
**Frontend:** HTML, CSS, JavaScript, AJAX, Bootstrap  
**Deployment & Version Control:** PythonAnywhere, GitHub  

---

## Installation & Getting Started

### 1. Clone the repository
Clone the repository to your local machine and navigate into the project folder:
```bash
git clone [https://github.com/2889073s/University_Marketplace.git](https://github.com/2889073s/University_Marketplace.git)
cd University_Marketplace
```

### 2. Create and activate a virtual environment
We use an isolated environment so it doesn’t affect global installs. The environment for this project is named `WADenv`.
```bash
conda create -n WADenv python=3.11
conda activate WADenv 
```

### 3. Install requirements
Install all required dependencies (including Django 2.2.28 and Pillow 12.1.0):
```bash
pip install -r requirements.txt
```
> **Tip:** If you change the requirements during development, you can update the text file by running `pip freeze > requirements.txt`.

### 4. Migrate and run the server
Set up the database and launch the local server:
```bash
python manage.py migrate
python manage.py runserver
```
> **VS Code Tip:** Ensure your interpreter is set correctly. Press `Shift + Cmd + P`, type "Python: Select Interpreter", and choose `Python 3.11.14 (WADenv)`.

### 5. Populate database & test (Optional but recommended)
To fill the database with sample data, run the population script. You will also want to create a superuser to access the Django admin dashboard.
```bash
python population_script.py
python manage.py test marketplace
python manage.py createsuperuser
```
> **Note:** All tests should pass successfully.

---


## Team 2D (LB02) Contributors
* **Daniel Thompson** (`3009940T`)
* **Skye Shields** (`2889073S`)
* **Josh Donald** (`3009507D`)
* **Tianqi Han** (`3075118H`)
* **Yuma Hayakawa** (`3070850H`)
