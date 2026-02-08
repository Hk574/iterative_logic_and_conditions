# Iterative Logic and Conditions
This repository focuses on repetitive execution patterns and conditional logic.

## Key Focus Areas
- Loops and iteration
- Nested conditions
- Logical checks
- Repetitive task handling

## Overview
Shows the ability to design solutions using iteration and conditional logic.

# Interactive Calculator with Multiprocessing Support

This project is an interactive command-line calculator that supports basic arithmetic operations. It allows users to perform calculations both with and without multiprocessing, enabling faster execution when running multiple calculations simultaneously.

## Features

- **Basic Arithmetic Operations**: Supports addition, subtraction, multiplication, and division.
- **Multiprocessing Support**: Enables calculations to run using separate processes, potentially improving performance for intensive computations.
- **Interactive REPL Mode**: Allows users to interact with the calculator using a Read-Eval-Print Loop (REPL) interface.
- **Error Handling**: Provides user-friendly messages for invalid inputs, division by zero, and unsupported operations.
- **Plugins System**: Supports dynamic loading of command plugins, making the system easily extensible.
- **Command-Line Arguments Support**: Users can perform operations directly from the command line or enable multiprocessing using a command-line argument (mp).
- **Automatic Timing**: Displays the time taken to perform each calculation.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- `pytest` for running tests
- Optional: `virtualenv` for creating a virtual environment

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/interactive-calculator.git
    cd interactive-calculator
    ```

2. Create a virtual environment (optional but recommended):

    ```bash
    python3 -m venv .venv
    source .venv/bin/activate  # On Windows: .venv\Scripts\activate
    ```

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

### Running the Calculator

You can run the calculator in REPL mode with or without multiprocessing.

1. **REPL Mode (Normal)**:

    ```bash
    python main.py
    ```

2. **REPL Mode with Multiprocessing Enabled**:

    ```bash
    python main.py mp
    ```

3. **Perform Calculation via Command Line**:

    ```bash
    python main.py 5 3 add
    ```

4. **Perform Calculation via Command Line with Multiprocessing**:

    ```bash
    python main.py mp 5 3 add
    ```

5. **Using Environment Variable to Enable Multiprocessing**: You can set the `USE_MULTIPROCESSING` environment variable to "true" to always use multiprocessing:

    ```bash
    export USE_MULTIPROCESSING=true
    python main.py
    ```

## Supported Commands

- **add**: Adds two numbers
- **subtract**: Subtracts the second number from the first
- **multiply**: Multiplies two numbers
- **divide**: Divides the first number by the second
- **square**: Finds the square of the number
- **cube**: Finds the cube of the number

## How to Use the REPL Mode

1. Start the Calculator:

    ```bash
    python main.py
    ```

2. **Commands Format**:

    For binary operations (add, subtract, multiply, divide): `<number1> <number2> <operation>`

    Example: `5 3 add`

    For single-operand commands (square, cube, etc. if added later): `<number> <operation>`

    Example: `9 square`

3. **Special Commands**:

    - `menu`: Displays the list of available commands.
    - `exit`: Exits the calculator.
