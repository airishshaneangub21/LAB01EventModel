# Paradigm Comparison

## Procedural Approach

In a procedural approach, the program follows a sequence of instructions.
The main program controls the order of operations.
The code may read the search input, validate it, send the request, and process the result step by step.
The program owns the main flow of execution.
Async results are handled when the program reaches the appropriate operation or callback.

## Object-Oriented Programming Approach

In OOP, the search functionality can be organized into classes and objects.
A SearchForm or SearchService object can contain the data and methods needed for searching.
Handlers and related operations can be placed inside appropriate classes or components.
The objects manage their own responsibilities while working together.
Async search results can be handled by methods, callbacks, or promises belonging to the objects.

## Event-Driven Approach

In an event-driven approach, the program responds to events such as form submission or button clicks.
The browser or event system controls when the handlers are called.
The search form has an event handler that starts the search when the user submits the form.
Handlers are registered and executed when their corresponding events occur.
Async results can arrive through Promises, callbacks, or other events without blocking the user interface.
