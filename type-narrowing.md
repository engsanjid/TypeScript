# Type Narrowing in TypeScript

## Introduction
Type narrowing is a core TypeScript mechanism that allows you to refine a variable's broad type into a more specific type within a conditional block. By examining runtime checks, TypeScript guarantees safer property and method access without unsafe casting.

## Practical Examples
TypeScript supports several narrowing techniques, including typeof, instanceof, and the in operator.

```typescript
function formatValue(input: string | number): string {
  if (typeof input === "string") {
    return input.toUpperCase();
  }
  return input.toFixed(2);
}

class Dog {
  bark(): string { return "Woof"; }
}

function handleAnimal(animal: Dog | Date): string {
  if (animal instanceof Dog) {
    return animal.bark();
  }
  return animal.toISOString();
}
```

The in operator checks for specific property existence on object unions, making control flow analysis extremely flexible across different shapes.

## Conclusion
Mastering type narrowing enables developers to write highly dynamic yet statically safe code. It bridges the gap between JavaScript's dynamic nature and TypeScript's compile-time safety guarantees.