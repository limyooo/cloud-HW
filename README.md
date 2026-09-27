# Cloud HW - CI Workflow Foundation

This repository serves as a foundational project for cloud computing assignments, featuring a modular Python calculator, automated test suites, and a fully configured GitHub Actions CI pipeline.

## Project Structure

```text
cloud-HW/
├── .github/
│   └── workflows/
│       └── ci.yml
├── src/
│   └── calculator.py
├── tests/
│   └── test_calculator.py
├── requirements.txt
└── README.md
```

## Prerequisites
- Python 3.8 or higher
- Git

## Running Tests Locally
To run the test suite on your local machine, follow these steps:
1. Install dependencies:
```text
pip install -r requirements.txt
```

3. Run tests with pytest:
```text
PYTHONPATH=. pytest
```

CI/CD Pipeline
The project utilizes GitHub Actions for continuous integration. Every time you push code to the repository or trigger it manually via workflow dispatch (ad-hoc), the workflow automatically:
1. Sets up the Python environment.
2. Installs required dependencies (pytest).
3. Executes the test suite to ensure code health.
