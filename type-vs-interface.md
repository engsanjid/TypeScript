# Type Aliases vs Interfaces in TypeScript

## Introduction
When developing robust applications in TypeScript, defining the shape of objects and data structures is fundamental. TypeScript provides two powerful constructs for this purpose: type aliases and interface declarations. While they often appear interchangeable, understanding their core differences helps developers write cleaner, more maintainable code.

## Core Differences
A type alias can name any type, including primitives, unions, tuples, and intersections, using the assignment operator. Conversely, an interface is specifically designed to declare the shape of object-oriented structures. 

```typescript
type UserID = string | number;

interface User {
  id: UserID;
  name: string;
}
```

Interfaces support declaration merging, meaning multiple declarations with the same name automatically combine their property definitions. Type aliases, however, will throw a duplicate identifier error if declared twice in the same scope.

## When to Choose One Over the Other
Use interface when defining object shapes or class contracts, especially if library extension or declaration merging is needed. Use type aliases when working with union types, tuples, primitives, or complex mapped types.

## Conclusion
Both type aliases and interfaces are indispensable tools in TypeScript. Choosing the right one depends heavily on whether you need declaration merging and union capabilities or strict object structures.