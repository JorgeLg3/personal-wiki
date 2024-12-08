From minudev [youtube tutorial](https://www.youtube.com/watch?v=xtp_DuPxo9Q)

# Typescript basic
```javascript
const a: number = 3
const b: string = 'hello'
const c: boolean = true
```

# Function notation
```javascript
const newFunction = (a: number, b: string): number => {
    // do something
    // ...
    return someNumber
}
```

# Arrays
```javascript
const option1: number[] = [1, 2, 3]
const option2: Array<number> = [1, 2, 3]
```

# any
TypeScript also has a special type, any, that you can use whenever you don’t want a particular value to cause typechecking errors.
```javascript
let obj: any = { x: 0 }
```

# Object types
```javascript
const a: {x: number; y: number} = {2, 3}
```
## Optional properties
```javascript
function printName(obj: { first: string; last?: string }) {
  // ...
}
// Both OK
printName({ first: "Bob" });
printName({ first: "Alice", last: "Alisson" });
```

# Union types
```javascript
let id: number | string = 'x5d'
id = 12
```

# Type aliases
```javascript
type Point = {
  x: number;
  y: number;
}
const a: Point = {2, 3}
```

# Type literals
```javascript
type Operation = 'multiply' | 'add' | 'divide' 
const a: Operation = 'multiply' // valid
const b: Operation = 'abs' // invalid
```