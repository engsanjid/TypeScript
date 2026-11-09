# B8A1 - Assignment 1: Problem Solving with TypeScript & OOP

## Overview

This assignment focuses on core TypeScript concepts, including:

- Advanced type narrowing and union types.
- Readonly tuples and generic rest parameters.
- Interface definitions, generic type mapping (`keyof`), and object-oriented programming with access modifiers (`private`, `protected`).
- Asynchronous programming with Promises and error handling.

All 8 problems are implemented in `solutions.ts`.

## Problems Solved

1. `multiplyValue` - Optional and default parameters
2. `processInput` - Union types and type narrowing
3. `formatCoordinate` - Readonly tuple
4. `concatenateArrays` - Generics and rest parameters
5. `getPopularCourses` - Interface and filtering
6. `pluckValues` - Generics with `keyof`
7. `Employee` and `Manager` - OOP, inheritance and access modifiers
8. `validateAgeAsync` - Promise and async error handling

## Blogs

- [Type Aliases vs Interfaces in TypeScript](./type-vs-interface.md)
- [Type Narrowing in TypeScript](./type-narrowing.md)

## File Structure

```
├── solutions.ts
├── type-vs-interface.md
├── type-narrowing.md
└── README.md
```

## How to Run

```bash
npx tsc solutions.ts --ignoreConfig
node solutions.js
```
