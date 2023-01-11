A to-do list that sorts tasks by deadlines (ordered and dated by month-day).

### Setup

Activate the environment (macOS/Linux)

```console
$ source . venv/bin/activate
```

Activate the environment (Windows)

```console
$ source . venv\Scripts\activate
```

Install Requirements

```console
$ pip install -r requirements.txt
```

Run the app

```console
$ flask run
```

### Description

Users are able to create new tasks with title and deadline, mark them as complete or incomplete, and to delete them as well.

The template uses Jinja2 syntax to loop through the list of to-do items and displays the title, deadline, and completion status of each item. It also includes links to update or delete the item.

Data is stored through SQLAlchemy and SQLite database. The application is configured to connect to a SQLite database named "db.sqlite". The app has routes for handling the different actions (creating, reading, updating, and deleting).

It's worth noting that SQLite Database is a lightweight file-based database, which is good for small-scale and development use cases. However, it's not suggested to use it in production.
