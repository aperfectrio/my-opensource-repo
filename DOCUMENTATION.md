# Project Documentation

## 📌 Overview

This project is a Python-based simulation of a **MediaWiki Community Manager system**.
It allows users to register developers, assign roles based on experience, allocate tasks, and generate a final report of contributors.

---

## 🎯 Purpose
* Practice GitHub workflow (repository, commits, branching)
* Understand open-source project structure
* Demonstrate Python concepts such as functions, loops, conditionals, and variable arguments

---

## ⚙️ Program Explanation
### 1. Welcome System (`welcome_developer`)
This function:

* Takes developer name and role as input
* Converts the role into uppercase as a badge
* Displays a formatted welcome message

👉 Purpose: Simulates onboarding of a contributor in an open-source project
---
### 2. Task Assignment (`assign_task`)
This function:
* Assigns a task based on developer role using `match-case`
* Example:

  * Junior Developer → Fix typo or formatting issues
  * Active Developer → Review pull requests
  * Senior Developer → Fix bugs
  * Lead Developer → Design features
  * Default → Read CONTRIBUTING guidelines

👉 Purpose: Represents real-world task distribution in open-source teams

---

### 3. Skills Handling (`check_skills`)
This function:
* Uses `*args` to accept multiple skills
* Prints each skill and total number of skills

👉 Purpose: Demonstrates flexible argument handling in Python

---

### 4. Main Program Flow
#### 🔹 User Input Loop
* Continuously asks for:
  * Developer name
  * Experience level (beginner, intermediate, advanced, expert)
* Name validation:
  * If invalid → assigns default name `"User"`

* Experience mapping:
  * beginner → Junior Developer
  * intermediate → Active Developer
  * advanced → Senior Developer
  * expert → Lead Developer
  * others → Observer

* Calls:
  * `welcome_developer()`
  * `assign_task()`
* Stores developer names in a list

---

#### 🔹 Loop Control
* User decides whether to continue or stop
* Loop exits when user inputs `"no"`

---

### 5. Predefined Entries
After input:
* Adds:
  * `"Anonymous"`
  * `"Vandal"`
  * `"Sara"`
👉 Purpose: Used to demonstrate filtering and control flow logic

---

### 6. Developer List Processing
The program scans the list:
* Skips `"Anonymous"` (using `continue`)
* Stops execution if `"Vandal"` is found (using `break`)
* Prints verified developers
👉 Purpose: Demonstrates loop control (`break`, `continue`)

---

### 7. Character Iteration
* Iterates through the string `"MediaWiki"`
* Prints each character separately
👉 Purpose: Demonstrates string iteration

---

### 8. Report Generation (`generate_report`)
This function:
* Takes project name and developer list (`*args`)
* Displays:
  * Project name
  * Total developers
  * List of developers
👉 Purpose: Simulates a summary report in a project

---

### 9. Final Execution
* Calls:
  * `generate_report()`
  * `check_skills()`
👉 Outputs final project report and skill summary

---

## 🛠 Technologies Used
* Python 3.x
* Git & GitHub
* Markdown

---

## 📂 Project Structure

* README.md: Provides an overview of the project, its purpose, and instructions on how to run the program.
* CONTRIBUTING.md: Guidelines for contributors, including setup instructions, contribution workflow, coding standards, and pull request process.
* LICENSE: Specifies the legal terms under which the project can be used, modified, and distributed.
* DOCUMENTATION.md: Contains detailed explanations of the program logic, structure, and functionality.
* 24013656_AHAMMED_TANIM.py: Main Python script implementing the developer management system.

---

## ▶️ How It Works (Summary)

1. User inputs developer details
2. System assigns role and task
3. Developers are stored and processed
4. Special cases (Anonymous, Vandal) are handled
5. Final report is generated
6. Skills are displayed

---

## 🌱 Future Improvements

* Add graphical user interface (GUI)
* Store developer data in a file or database
* Improve input validation (allow spaces in names)
* Expand role and task system

---

## 🤝 Contribution

Refer to CONTRIBUTING.md for contribution guidelines.

---

## 📄 License

This project is licensed under the MIT License.
