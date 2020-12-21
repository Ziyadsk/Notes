# TypeScript

### tsc command
`tsc [FILE_NAME]` to check and compile to a js file

`--watch` flag tells typeScript to watch for changes and recompiles automaticly instead of running tsc every time we make a change.

### basic types
string
never 
unknown
number
any
boolean
null

### Arrays & tuples

### Union types

### return **types**

### Type alias 
type myType = number; 

### Interfaces
#### Combine multiple interfaces
`&`
### enums
```ts
enum Color {
    Red,
    Green,
    Blue
}
```
### Type casting


### Classes
#### Constructor
#### Access modifiers


### Generics

### TsConfig



#### Compiler options**
"outDir" : specifies where** to put the compiled js
"rootDir" : specifies the dir you want to get your ts files from 
"noEmitOnError": do not generate js files when there is an error
"strict" : "keep the best type checking stuff"