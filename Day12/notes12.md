### **1. Basics of Functions**

A function is a reusable block of code that performs a specific task when called. Functions are useful to organize code, make it reusable, and reduce redundancy.

---

### **2. Defining a Function**

You define a function using the `def` keyword followed by the function name, parentheses, and a colon `:`.

#### **Syntax**:
```python
def function_name(parameters):
    # Block of code
```

#### **Example**: Basic function to greet a user
```python
def greet():
    print("Hello! Welcome to the Python course.")
greet()
```

**Output**:
```
Hello! Welcome to the Python course.
```

---

### **3. Function Parameters**

Parameters are variables used to pass data into a function.

#### **Example**: Function with a parameter
```python
def greet_user(name):
    print(f"Hello, {name}! Welcome to the Python course.")

greet_user("Anand")
```

**Output**:
```
Hello, Anand! Welcome to the Python course.
```

---

### **4. Returning Values from a Function**

A function can return a value using the `return` keyword, which allows the output of the function to be reused elsewhere.

#### **Example**: Function that adds two numbers and returns the result
```python
def add_numbers(a, b):
    return a + b

result = add_numbers(10, 20)
print("The sum is:", result)
```

**Output**:
```
The sum is: 30
```

---

### **5. Default Parameter Values**

You can define a default value for a parameter, which is used if no argument is passed when the function is called.

#### **Example**: Function with a default parameter
```python
def greet(name="Student"):
    print(f"Hello, {name}! Welcome to the Python course.")

greet()  # Uses default value "Student"
greet("Geetha")  # Uses passed value "Geetha"
```

**Output**:
```
Hello, Student! Welcome to the Python course.
Hello, Geetha! Welcome to the Python course.
```
Here are the sections for **Nested Functions** and **Local/Global Variables**:

---

### **6. Local and Global Variables**

- **Local Variables** are defined inside a function and are only accessible within that function.
- **Global Variables** are defined outside all functions and are accessible from anywhere in the code.

#### **Example**: Local vs Global variables
```python
name = "Global Name"

def greet():
    name = "Local Name"
    print(name)

greet()  # Prints local variable
print(name)  # Prints global variable
```

**Output**:
```
Local Name
Global Name
```

In this example, the local variable `name` inside the function does not affect the global variable `name`.

---

### **Assignment**:
1. **Greet Function**: Write a function `greet()` that takes no arguments and prints a greeting message.
2. **Parameterized Greet**: Write a function `greet_user()` that takes a name as input and prints a custom greeting.
3. **Sum Function**: Write a function `add_numbers(a, b)` that returns the sum of two numbers. Call this function with different values.
