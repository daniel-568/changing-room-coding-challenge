A to-do list that sorts tasks by deadlines (for simplicity's sake - dated by month-day agnostic to the year and hour/minutes/seconds).

### Setup
Create project with virtual environment
```console
$ mkdir myproject
$ cd myproject
$python3 -m venv venv
```

Activate it (Linux)
```console
$ . venv/bin/activate
```

Install Requirements
```console
pip install -r requirements.txt
```

Run the app
```console
$ flask run
```

Users are able to create new tasks with title and deadline, mark them as complete or incomplete, and to delete them as well.

Data is stored through SQLAlchemy and SQLite database.