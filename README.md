# OOP in Python

This project contains a Jupyter Notebook (`oop_in_python.ipynb`) that explains and demonstrates the core principles of Object-Oriented Programming (OOP) in Python, including composition, inheritance, encapsulation, and polymorphism. The notebook includes theoretical explanations as well as practical examples.

## Project Structure

- `oop_in_python.ipynb`: Jupyter Notebook containing explanations and code examples for OOP principles in Python.

## Prerequisites

To run the notebook, you need to have Python and Jupyter Lab installed. It's recommended to use a virtual environment to manage dependencies.

## Installation

1. **Clone the repository:**
    ```sh
    https://github.com/alexey-krasnov/oop_in_python.git
    cd oop_in_python
    ```

2. **Create a virtual environment:**
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required packages:**
    ```sh
    pip install -r requirements.txt
    ```

4. **Start Jupyter Lab:**
    ```sh
    jupyter lab
    ```

5. Open the `oop_in_python.ipynb` notebook and run the cells.

## OOP Principles Covered

### Composition

Composition is a principle that allows one object to contain other objects as its components. It represents a "has-a" relationship and enables the creation of complex objects from simpler ones.

**Example:**

```python
class Engine:
    def __init__(self, horsepower):
        self.horsepower = horsepower

    def start(self):
        print(f"Engine with {self.horsepower} horsepower started")

class Car:
    def __init__(self, make, model, engine):
        self.make = make
        self.model = model
        self.engine = engine

    def start(self):
        print(f"{self.make} {self.model} is starting...")
        self.engine.start()

engine = Engine(150)
car = Car("Toyota", "Corolla", engine)
car.start()


## Author

[Dr. Aleksei Krasnov](https://github.com/alexey-krasnov)
email: alexeykrasnov1989@gmail.com

Feel free to contribute, report issues, or provide feedback!

## License
This project is licensed under the MIT - see the LICENSE.md file for details.