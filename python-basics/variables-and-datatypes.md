# Learning Variables and Data Types in Python

## **1. What are Variables?**

- Variables are containers for storing data values.
- In Python, you dont need to declare a variable type explicitly; it is inferred based on the value assigned.

### **Syntax**

```python
variable_name = value
```

### **Examples**

```python
x = 10          # Integer
name = "John"   # String
is_active = True # Boolean
```

---

## **2. Rules for Naming Variables**

- Variable names can only contain **letters, numbers, and underscores** (e.g., `my_variable`).
- Variable names **cannot start with a number** (e.g., `2variable` is invalid).
- Variable names are **case-sensitive** (e.g., `Age` and `age` are different).
- Avoid using **Python reserved keywords** (e.g., `if`, `for`, `while`).

---

## **3. Data Types in Python**

Python provides several built-in data types to handle different kinds of data.

### **3.1 Numeric Types**

- **int**: Integer values.

  ```python
  x = 100
  ```

- **float**: Decimal numbers.

  ```python
  y = 3.14
  ```

- **complex**: Complex numbers.

  ```python
  z = 2 + 3j
  ```

### **3.2 Sequence Types**

- **str**: Text data.

  ```python
  name = "Hello, World!"
  ```

- **list**: Ordered, mutable collection.

  ```python
  fruits = ["apple", "banana", "cherry"]
  ```

- **tuple**: Ordered, immutable collection.

  ```python
  coordinates = (10, 20)
  ```

- **range**: Sequence of numbers.

  ```python
  numbers = range(5)  # 0, 1, 2, 3, 4
  ```

### **3.3 Set Types**

- **set**: Unordered, unique items.

  ```python
  unique_numbers = {1, 2, 3}
  ```

- **frozenset**: Immutable version of a set.

  ```python
  frozen_set = frozenset([1, 2, 3])
  ```

### **3.4 Mapping Type**

- **dict**: Key-value pairs.

  ```python
  person = {"name": "Alice", "age": 25}
  ```

### **3.5 Boolean Type**

- **bool**: Represents `True` or `False`.

  ```python
  is_logged_in = True
  ```

### **3.6 Binary Types**

- **bytes**: Immutable sequence of bytes.

  ```python
  byte_data = b"hello"
  ```

- **bytearray**: Mutable sequence of bytes.

  ```python
  mutable_bytes = bytearray(b"hello")
  ```

- **memoryview**: View of memory from another binary object.

  ```python
  mv = memoryview(bytes(5))
  ```

### **3.7 None Type**

- **NoneType**: Represents no value.

  ```python
  x = None
  ```

---

## **4. Checking Data Types**

Use the `type()` function to check the data type of a variable.

### **Example**

```python
x = 10
print(type(x))  # Output: <class 'int'>
```

---

## 5. Type Conversion

Convert one data type to another using type conversion functions:

- `int()`: Converts to an integer.
- `float()`: Converts to a float.
- `str()`: Converts to a string.
- `list()`: Converts to a list.

### **Type Conversion Examples**

```python
x = "123"
y = int(x)  # Converts string "123" to integer 123
z = float(y)  # Converts integer 123 to float 123.0
```

---

## **6. Mutable vs Immutable Data Types**

- **Mutable**: Can be changed after creation.
  - Examples: `list`, `dict`, `set`, `bytearray`
- **Immutable**: Cannot be changed after creation.
  - Examples: `int`, `float`, `str`, `tuple`, `frozenset`, `bytes`

### **Mutable vs Immutable Data Type Example**

```python
# Mutable
my_list = [1, 2, 3]
my_list[0] = 10  # Allowed

# Immutable
my_tuple = (1, 2, 3)
my_tuple[0] = 10  # Raises an error
```

---

## **7. Best Practices**

- Use descriptive variable names.

  x = 10            # Not descriptive
  age_of_student = 10  # Descriptive

- Follow PEP 8 style guidelines.
- Keep variable types consistent when possible.

---

## **8. Practice Exercises**

1. Create variables of different data types and print their types using `type()`.
2. Convert a string to an integer, then to a float.
3. Create a list and modify one of its elements.
4. Try to modify a tuple and observe the error.

Happy Coding!
