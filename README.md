# Translating Ruby to Javascript

This is my personal reference / infodump / cheatsheet for translating the concepts and techniques I have learned in Ruby to Javascript

## Contents

1. [Variables](#Variables)
2. [Conditionals](#Conditionals)
    * If
    * Else
    * Else If
    * Unless
    * Case
3. [Loops](#Loops)
    * While
    * Until
4. [Iteration](#Iteration)
    * Each
    * Map
5. [Methods](#Methods)
6. [Classes](#Classes)

#

### 1.
## Variables

### In Ruby:

Variables are simply assigned with the equals sign. By default variables are only available within the scope under which they were defined, and can be reassigned whenever within that scope.

```
cat = 'Rufus'
```

### In Javascript:

There are three ways of assigning variables

Old style variable assignment using `var` creates a variable which is mutable and, by default, globally accessible.

DON'T bother with it.

```
var dog = 'Mable'
```

New style variable assignment uses the keywords `const` and `let` and these variables are only accesible from the scope in which they are defined.

`const` can not be reassigned after is is created, try to use it unless you _need_ to do otherwise.

```
const sphereEulerCharacteristic = 2
```

`let`, however, can be reassigned at any time within its scope. This is the closest thing in Javascript to a plain Ruby variable

```
let childHeight = 160
```



#

### 2.
## Conditionals

### In Ruby:

The conditional keywords in Ruby are `if`, `else`, `elsif`, and `unless`

A conditional statement is opened using `if` or `unless` and closed with the `end` keyword.

```
if time == morning
  meal = breakfast
elsif time == noon
  meal = lunch
else
  meal = dinner
end
```

### In Javascript:

The conditional keywords are `if`, `else` and the phrase `else if`. There is no unless. The condition itself is in parentheses and the block to be executed is in curly brackets, like so:

```
if (itIsCold()) {
  outerwear = "coat";
} else if (itIsMild()) {
  outerwear = "shacket";
} else {
  outerwear = "none";
}
```

#

### 3.
## Loops

### In Ruby:

### In Javascript:

#

### 4.
## Iteration

### In Ruby:

### In Javascript:

#

### 5.
## Methods

### In Ruby:

### In Javascript:

#

### 6.
## Classes

### In Ruby:

### In Javascript
