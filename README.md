# Uninitialized Property Access in C#

This repository demonstrates a common error in C#: accessing a property before it's been assigned a value. This often leads to `NullReferenceException` runtime errors.

## The Bug
The `bug.cs` file contains a class with a property that is not explicitly initialized in the constructor.  When `MyMethod` attempts to use this property, a `NullReferenceException` occurs if the property is null.

## The Solution
The `bugSolution.cs` file shows how to properly initialize the property, either in the constructor or by assigning a default value.