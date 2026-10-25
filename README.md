# DevOps Mini Project

A beginner-friendly DevOps project demonstrating Python development, unit testing, Docker containerization, Git version control, and continuous integration with GitHub Actions.

## Features

- Python application with an addition function
- Unit tests using Python's built-in `unittest` framework
- Docker image built using a lightweight Python base image
- Automated testing and application execution with GitHub Actions
- Git-based version control and GitHub repository hosting

## Project Structure

```text
devops-mini-project/
├── .github/
│   └── workflows/
│       └── python-ci.yml
├── app.py
├── test_app.py
├── Dockerfile
├── .gitignore
└── README.md
```

## Requirements

- Python 3.12 or compatible Python 3 version
- Docker Desktop or Docker Engine
- Git

## Run the Application

Clone the repository:

```bash
git clone https://github.com/priyanshudas81442-Prider/devops-mini-project.git
cd devops-mini-project
```

Run the application:

```bash
python3 app.py
```

Expected output:

```text
Welcome to my DevOps Mini Project!
2 + 3 = 5
```

## Run Unit Tests

Run:

```bash
python3 -m unittest -v
```

The tests verify addition with positive and negative integers.

## Build and Run with Docker

Build the image:

```bash
docker build -t devops-mini-project:1.0 .
```

Run the container:

```bash
docker run --rm devops-mini-project:1.0
```

The container runs the Python application and displays its output.

## Continuous Integration with GitHub Actions

The workflow is located at `.github/workflows/python-ci.yml`.

Whenever code is pushed to the `main` branch, GitHub Actions automatically:

1. Checks out the repository.
2. Sets up Python 3.12.
3. Runs the unit tests.
4. Executes the application.

The workflow also runs for pull requests targeting `main`.

## Skills Demonsrated

Python · Unit Testing · Docker · Git · GitHub · GitHub Actions · CI

## Author

Created as a hands-on project while learning DevOps fundamentals.
