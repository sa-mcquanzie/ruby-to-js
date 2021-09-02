# Translating Ruby to Javascript

This is my personal reference / infodump / cheatsheet for translating the concepts and techniques I have learned in Ruby to Javascript

## Contents

1. [Variables](#Variables)
2. [Conditionals](#Conditionals)
    * If
    * Else
    * Else If
    * Unless
    * Ternary
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

### a. `if`, `else` and `elif`

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
In Ruby, unlike in Javascript, for simple cases with only one branch, you can also choose to invert the if statement, like so

```
snack if hungry_between_mealtimes
```

which is quite lovely.

### In Javascript:

The conditional keywords are `if`, `else` and the phrase `else if`. There is no unless. The conditional is in parentheses and the clauses are in curly brackets, like so

```
if (itIsCold()) {
  outerwear = "coat"
} else if (itIsMild()) {
  outerwear = "shacket"
} else {
  outerwear = "none"
}
```

### b. Ternary Expressions

The syntax for a ternary expression is identical in both languages

### In Ruby:

```
material = fancy ? 'silk' : 'polyester' 
```

### In Javascript:

```
let stone = loaded ? "diamond" : "cubicZirconia"
```

Unlike in Ruby, you can go wild with ternary chaining as follows

```
return num % 15 == 0 ? "fizzbuzz"
    : num % 3 == 0 ? "fizz"
    : num % 5 == 0 ? "buzz"
    : `${num}`
```

and even nest them

```
return num % 3 == 0
    ? num % 5 == 0 
        ? "fizzbuzz"
        : "fizz"
    : num % 5 == 0
        ? "buzz"
        : `${num}`
```

although I think you probably *shouldn't*.

### c. Case / Switch statements

### In Ruby:

```
arche = case philosopher
when 'Thales'
  :water
when 'Anaximenes'
  :air
when 'Anaximander'
  :void
when 'Heraclitus'
  :flux
else
  :mystery
end
```

### In Javascript:

```
switch (powerpuff) {
  case "Blossom":
    colour = "#ffcccc";
    break;
  case "Bubbles":
    colour = "#99ccff";
    break;
  case 'Buttercup':
    colour = "#bbff99";
    break;
  default:
    colour = "#000000";
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
