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
- python decorators allows to modify or extend the behavioural function or method without changing its source code
'''
def my_decorator(func):
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
'''
