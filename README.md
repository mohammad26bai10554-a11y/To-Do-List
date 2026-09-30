# To-Do-List
# 📝 Todo List — Python

A simple **command-line Todo List application** built using Python.
This project allows users to add, view, and delete tasks through an interactive menu.

## 📌 Features

* ➕ Add new tasks
* 👀 View all available tasks
* 🗑️ Delete tasks by task number
* 🚫 Prevents empty tasks from being added
* ⚠️ Handles invalid menu choices
* 🚪 Exit the application safely

## 🛠️ Technologies Used

* **Python 3**
* Python built-in functions
* Lists
* Functions
* Loops
* Conditional statements
* User input

No external libraries are required.

## 📂 Project Structure

```text
Todo-List/
│
├── todo.py
└── README.md
```

> `todo.py` contains the main Todo List application.

## 🚀 Getting Started

### Prerequisites

Make sure Python 3 is installed on your computer.

You can check your Python version using:

```bash
python --version
```

or:

```bash
python3 --version
```

## 📥 Installation

1. Clone or download this repository.

2. Open a terminal in the project directory.

3. Run the Python program:

```bash
python todo.py
```

If your system uses `python3`, run:

```bash
python3 todo.py
```

## ▶️ How to Use

When the program starts, you will see:

```text
===== TODO LIST =====
1. Add Task
2. View Tasks
3. Delete Task
4. Exit

Enter your choice:
```

### 1. Add Task

Select option `1` and enter the task you want to add.

Example:

```text
Enter your choice: 1
Enter a new task: Complete Python homework
Task added successfully!
```

### 2. View Tasks

Select option `2` to display all tasks.

Example:

```text
--- Todo List ---
1 . Complete Python homework
2 . Read a book
3 . Practice programming
```

### 3. Delete Task

Select option `3` and enter the number of the task you want to delete.

Example:

```text
Enter task number to delete: 2
Deleted: Read a book
```

### 4. Exit

Select option `4` to close the program.

```text
Thank you for using Todo List!
```

## 🧠 How the Code Works

The program stores tasks inside a Python list:

```python
tasks = []
```

### `show_tasks()`

Displays all tasks currently stored in the list.

```python
def show_tasks():
```

If there are no tasks, it displays:

```text
No tasks available.
```

Otherwise, it uses `enumerate()` to display each task with a number.

### `add_task()`

Gets a task from the user and adds it to the `tasks` list.

The program also checks whether the user entered an empty task:

```python
if task.strip() == "":
```

Empty tasks are rejected.

### `delete_task()`

Displays the current tasks and asks the user which task they want to delete.

The selected task is removed using:

```python
tasks.pop(number - 1)
```

`number - 1` is used because Python lists start counting from index `0`, while the Todo List displays task numbers starting from `1`.

### Main Menu

The program continuously displays the menu using:

```python
while True:
```

The loop continues until the user chooses option `4`.

## ⚠️ Current Limitations

This is a simple beginner-level Todo List application. Some limitations include:

* Tasks are stored only in memory.
* All tasks are lost when the program is closed.
* Entering non-numeric input when deleting a task can cause an error.
* Tasks cannot currently be edited or marked as completed.
* There is no database or file storage.

## 🔮 Possible Future Improvements

The project could be extended with:

* ✅ Mark tasks as completed
* ✏️ Edit existing tasks
* 💾 Save tasks to a file
* 📂 Load saved tasks when the program starts
* 📅 Add due dates
* 🔍 Search tasks
* 🗂️ Organize tasks into categories
* 🛡️ Add better input validation
* 🖥️ Create a graphical user interface (GUI)

## 🎯 Learning Objectives

This project is useful for learning the fundamentals of Python, including:

* Variables
* Lists
* Functions
* `if/elif/else` statements
* `while` loops
* `for` loops
* `enumerate()`
* `input()`
* String methods
* List methods such as `append()` and `pop()`

## 📄 License

This project is free to use, modify, and learn from.

---

Name: Mohammad Absar Hussain
Registration No.: 26BAI10554

A beginner-friendly Python Todo List project created for practicing basic Python programming concepts.

