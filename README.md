# TestSuite

## Overview

**TestSuite** is a comprehensive tool designed to assist developers in writing unit tests and docstrings for their code. By leveraging the Google Gemini API with the `dspy` library, TestSuite generates accurate and relevant docstrings and unit tests based on the provided code and expected output. Additionally, it measures code coverage and provides detailed coverage reports to ensure the effectiveness of your test cases.

## Features

- **Docstring Generation**: Automatically generate docstrings for your code based on the given code and expected output.
- **Unit Test Creation**: Create unit tests that validate the correctness of your code against the expected output.
- **Coverage Reporting**: Generate detailed reports on test coverage to identify untested code and improve overall test quality.  
## Technologies

- **Frontend**: React
- **Backend**: Django
- **AI Integration**: Google Gemini API with `dspy` library

## Getting Started

### Prerequisites

- Node.js and npm (for React frontend)
- Python and Django (for backend)
- Google Gemini API credentials
- `dspy` library for interacting with Google Gemini

### Website link

  ```bash
   https://testsuite-1.onrender.com/
  ```
###
Sample Input for Code Coverage:

  ```bash
def add(a, b):
    return a + b
def subtract(a, b):
    return a - b
def multiply(a, b):
    return a * b
    
class TestMyFunctions(unittest.TestCase):
    def test_add(self):
        self.assertEqual(add(2, 3), 5)
        self.assertEqual(add(-1, 1), 0)
        self.assertEqual(add(0, 0), 0)
    def test_subtract(self):
        self.assertEqual(subtract(5, 3), 2)
        self.assertEqual(subtract(0, 4), -4)
        self.assertEqual(subtract(-3, -3), 0)
    def test_multiply(self):
        self.assertEqual(multiply(2, 3), 6)
        self.assertEqual(multiply(-1, 5), -5)
        self.assertEqual(multiply(0, 100), 0)
    def test_multiply_2(self):
        self.assertEqual(multiply(2, 3), 6)
        self.assertEqual(multiply(-1, 5), -5)
        self.assertEqual(multiply(0, 100), 0)
    ```bash
### OR

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/MoustaphaGh30/TestSuite.git
   cd testsuite
   ```

2. **Set up the backend:**

   ```bash
   cd backend
   python manage.py migrate
   python manage.py runserver
   ```

3. **Set up the frontend:**

   ```bash
   cd ../frontend
   npm install
   npm start
   ```

4. **Configure API keys:**

   - Create a `.env` file in the `backend` directory and add your Google Gemini API credentials.

### Usage

1. **Access the Frontend:**
   Open your web browser and navigate to `http://localhost`. Here, you can input your code and expected output to generate docstrings and unit tests.

2. **Generate Docstrings and Unit Tests:**
   - Enter your code and the expected output in the designated fields.
   - Click the "Generate" button to receive generated docstrings and unit tests.


## License

This project is licensed under the MIT License.
