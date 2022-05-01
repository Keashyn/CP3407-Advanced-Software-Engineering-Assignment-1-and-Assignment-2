# CP3407-Advanced-Software-Engineering-kangaroos-Assignmnet-1-and-Assignment-2

# Spendee-Tracker

A web app for tracking expenses and mangining users spending habits.

## Features

* Quick and bulk expensing
* Budget creation and automatic tracking of expenses per budget
* Custom spend categories
* Dashboard with dynamic reporting
* Detailed reports that break down spending
* Add additional payers for tracking expenses across multiple people
* Export your data directly into raw, CSV, and Excel
* Responsive design - compatible with all major browsers and devices

## Built with

* Front-end: [Bootstrap](https://getbootstrap.com/), [Chart.js](https://www.chartjs.org/), and [DataTables](https://datatables.net/)
* Back-end: [Flask](https://flask.palletsprojects.com)

## To install and run Spendee Tracker App
  
  1. Clone the repo:

    git clone https://github.com/CP3407-Advanced-Software-Engineering/CP3407-Advanced-Software-Engineering-kangaroos-Assignmnet-1-and-Assignment-2-Expense-Tracker-App


  2. Create your virtual environment:

    python -m venv env

  3. Activate your virtual environemnt

    env\Scripts\activate

  4. Install the packages in the following file:

    pip install -r requirements.txt

  5. Create a Database in Postgres

  * Install Postgres App for localhost
  * Install Postgres management app pgAdmin 4

These apps need to be installed on user computer first to make a database before connecting to the application in flask.
Once that has been done just follow the steps on how to configure with postgres app and pgAdmin 4 app on the user computer to create a database.
Then the user can use this scheme file named keashynnaidoo.session.sql to create tables in the database.

  6. To connect to the database that was created in Step 5

You will need this code to connect to the database:

engine = create_engine =("postgres+psycopg2://{user}:{password}@{hostname}:{port}/{database-name}")

User needs to replace these words in the above code with their computer details for localhost

* user - keashynnaidoo
* password - add password that you created for database or leave empty and say passowrd
* hostname - localhost
* port - 5432
* database-name - postgres

Then you will get something like this:

engine = create_engine("postgresql+psycopg2://keashynnaidoo:password@localhost:5432/postgres")

once that has been done you can go and paste it in these python files which are:

* app.py
* spendee_account.py
* spendee_budgets.py
* spendee_categories.py
* spendee_dashboard.py
* spendee_expenses.py
* spendee_reports.py

all these python file will be connected to the database.

  7. Build and run the FLASK app in VScode
