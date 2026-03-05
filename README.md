# GitHub Composite Action Demo

This project demonstrates how to create and use a **custom composite action** in GitHub Actions.
The action takes two input numbers (`number1` and `number2`) and calculates their sum during a CI workflow.

## 📌 Project Purpose

The purpose of this project is to show how a **GitHub composite action** can be created and integrated into a workflow to automate simple tasks.

## ⚙️ Features

* Custom composite action using `action.yml`
* Accepts input parameters
* Performs arithmetic operation (addition)
* Runs automatically using GitHub Actions CI workflow

## 📂 Project Structure

```
.github/
 ├── actions/
 │   └── add-numbers/
 │       └── action.yml
 │
 └── workflows/
     └── ci.yml
```

## 🧩 Inputs

| Input   | Description   |
| ------- | ------------- |
| number1 | First number  |
| number2 | Second number |

## ▶️ Example Usage

```
- name: Run Add Numbers Action
  uses: ./.github/actions/add-numbers
  with:
    number1: 5
    number2: 7
```

## 🧮 Output

The workflow prints the result of the addition in the GitHub Actions log.

Example output:

```
Result: 12
```

## 🚀 Technologies Used

* GitHub Actions
* YAML
* Bash scripting

## 👨‍💻 Author

Created as part of a CI/CD learning project.
