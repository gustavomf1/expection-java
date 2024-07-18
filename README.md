## Repository Purpose

### Class Summary

**Solution 1 (very poor): Validation logic in the main program**

- Validation logic is not delegated to the reservation

**Solution 2 (poor): Method returning a string**

- The operation's semantics are compromised
  - Returning a string is unrelated to updating a reservation
  - What if the operation needed to return a string?
- It is still not possible to handle exceptions in constructors
- There is still no compiler assistance: the programmer must "remember" to check for errors
- The logic is structured with nested conditionals

**Solution 3 (good): Exception handling**

## Learning Repository on Exception Handling

- **Throws clause**: propagates the exception instead of handling it

- **Throw clause**: throws the exception / "terminates" the method

- **Exception**: compiler forces handling or propagation

- **RuntimeException**: compiler does not force handling

- The exception handling model allows errors to be managed consistently and flexibly, using best practices

### Advantages:
- Delegated logic
- Constructors can handle exceptions
- Possibility of compiler assistance (Exception)
- Simpler code. There are no nested conditionals: whenever an exception is thrown, execution is interrupted and falls into the corresponding catch block.
- It is possible to capture other system exceptions as well776
