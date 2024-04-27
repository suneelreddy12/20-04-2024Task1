# Objects and Their Internal Representation in JavaScript

- In JavaScript, an object is a collection of key-value pairs, where each key is a unique identifier mapped to a corresponding value. Objects in JavaScript can represent various entities, such as real-world objects, data structures, and even functions

// Example of an object representing a person
let person = {
    name: "Suneel Reddy",
    age: 30,
    profession: "Full Stack Developer"
};

- In JavaScript, arrays are also objects. They inherit properties and methods from the Array prototype object, making them behave like specialized objects optimized for storing sequential data. Arrays offer additional functionality such as indexed access to elements and methods for manipulating arrays efficiently.

// Example of an array in JavaScript
let numbers = [1, 2, 3, 4, 5];

# Objects vs Primitive Values:
It's essential to distinguish between objects and primitive values (such as numbers, strings, and booleans) in JavaScript:

- Objects: Mutable and passed by reference. Changes to an object's properties affect all references to that object.
- Primitive Values: Immutable and passed by value. Assigning a primitive value to another variable creates a copy of the value, and changes to one variable do not affect the other.