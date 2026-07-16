# 50 Python Interview Questions

A comprehensive list of 50 Python interview questions categorized by topic. Use these questions to prepare for technical interviews or to gauge your proficiency.

## Table of Contents
1. [Core Python Concepts](#core-python-concepts)
2. [Object-Oriented Programming (OOP)](#object-oriented-programming-oop)
3. [Advanced Concepts & Concurrency](#advanced-concepts--concurrency)
4. [Data Structures & Built-ins](#data-structures--built-ins)
5. [Testing, Web, & Practical Development](#testing-web--practical-development)

---

### Core Python Concepts

1. What is the difference between a list and a tuple?
- lists are mutable and tuples are immutable
- tuples allocates less memory than list
- list [] brackets and tuple () brackets 
2. How is memory managed in Python?
- python stores all objects in private heap
- automated Garbage collection
- reference counting used to track how many reference point to them
3. What are Python decorators and how do you write a custom one?
  python decorators allows to modify or extend the behavioural function or method without changing its source code
- def my_decorator(func):
    def wrapper(*args,**kwargs):
        print("----")
        func(*args,**kwargs)
        print(args)
        print(kwargs)
        print("=====")
    return wrapper

@my_decorator
def say_ola(*args,**kwargs):
    print("Hello sir")

say_ola(idly="soft")

4. What is the difference between a deep copy and a shallow copy?
5. What are the formatting rules defined in PEP 8?
6. What is the difference between the `is` operator and the `==` operator?
7. What are Python generators and when should you use them?
8. What is a lambda function and what are its limitations?
9. How does Python's `try-except-else-finally` block handle exceptions?
10. What is the purpose of the `__init__` method in Python classes?

### Object-Oriented Programming (OOP)

11. How does Python handle multiple inheritance and what is the Diamond Problem?
12. What is Method Resolution Order (MRO) and how can you check it?
13. What are dunder or magic methods, and can you give three examples?
14. What is the practical difference between `@classmethod` and `@staticmethod`?
15. How do you implement data encapsulation and access modifiers in Python?
16. What is the purpose of the `super()` function?
17. How do you define and use an abstract class in Python?
18. How is polymorphism achieved in Python's dynamic typing system?
19. How do you implement a Singleton design pattern using the `__new__` method?
20. Why might you choose composition over inheritance in a Python project?

### Advanced Concepts & Concurrency

21. What is the Global Interpreter Lock (GIL) and how does it impact performance?
22. How do you bypass the GIL for heavy CPU-bound tasks?
23. What is the difference between the `threading` and `multiprocessing` modules?
24. How do the `async` and `await` keywords work under the hood in `asyncio`?
25. How do you create a custom context manager using a class or a decorator?
26. What is monkey patching and what are its risks?
27. How do `*args` and `**kwargs` handle variable numbers of function arguments?
28. What is a closure in Python and how do you implement one?
29. What are metaclasses and what is their primary use case?
30. What is variable shadowing and how can you access a shadowed global variable?

### Data Structures & Built-ins

31. What is the time complexity of looking up a key in a Python dictionary?
32. What is the difference between the `list.append()` and `list.extend()` methods?
33. How do you write list, dictionary, and set comprehensions?
34. How do Python sets guarantee that all elements are unique?
35. When would you use a `collections.defaultdict` instead of a standard dictionary?
36. What is the difference between `set.remove()` and `set.discard()`?
37. How do the built-ins `any()` and `all()` evaluate truthiness?
38. What does the `zip()` function do and how does it handle mismatched sequences?
39. How do iterators differ from iterables in Python?
40. What are the different ways to reverse a list or string, and which is fastest?

### Testing, Web, & Practical Development

41. How do you write and organize a unit test suite using `unittest` or `pytest`?
42. Why are virtual environments essential for Python development?
43. What are the structural architectural differences between Flask and Django?
44. How does an Object-Relational Mapper (ORM) protect against SQL injection?
45. What tools and techniques do you use to profile and optimize slow Python code?
46. How do you handle connection timeouts and status code validation with the `requests` library?
47. What is the exact difference in purpose between `__str__` and `__repr__`?
48. How do you safely serialize and deserialize JSON objects in Python?
49. Why should you store sensitive application secrets in environment variables?
50. How do you manage database schema changes and migrations in a production app?
