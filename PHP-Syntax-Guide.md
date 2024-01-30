#                   **Welcome**
##                PHP Syntax Guide
####                 Created by Grrham
##### This cheat sheet provides examples and explanations for fundamental PHP commands, covering essential topics such as variables, loops, arrays, and more.

### PHP Comments
Comments are used to add explanatory text within the code that is not executed. There are single-line comments using `//` and multi-line comments using `/* */`.

```bash
<?php
    // This is a single-line comment

    /*
        This is a multi-line comment.
        It can span multiple lines.
    */
?>
```

### PHP Variables
Variables are used to store information. Variable names start with a dollar sign `$` followed by the name. Variables in PHP are case-sensitive.

```bash
<?php
    $name = "John";
    $age = 25;

    echo "Name: $name, Age: $age";
?>
```

### PHP Echo / Print
Both `echo` and `print` are used to output data to the screen. echo is faster and can accept multiple parameters, while print can only accept one argument and returns 1.

```bash
<?php
    $variable = "You can include variables in echo statements.";

    echo $variable;
    echo "This outputs a string.";
    echo "<p>You can also include HTML in an echo statement.</p>";

    print "Print is used to output a string.";
?>
```
### PHP Data Types
PHP supports various data types including integers, floats, strings, booleans, arrays, and objects.
```bash
<?php
    $integerVar = 42;
    $floatVar = 3.14;
    $stringVar = "Hello, PHP!";
    $boolVar = true;
    $arrayVar = [1, 2, 3];
?>
```
### PHP Strings
Strings are sequences of characters. They can be declared using single or double quotes.
```bash
<?php
    $singleQuotes = 'This is a string with single quotes.';
    $doubleQuotes = "This is a string with double quotes.";

    $concatenation = $singleQuotes . " " . $doubleQuotes;
?>
```
### PHP Numbers
Numbers in PHP can be integers or floats. They can be used in mathematical operations.
```bash
<?php
    $integerNumber = 42;
    $floatNumber = 3.14;

    $result = $integerNumber + $floatNumber;
?>
```
### PHP Constants
Constants are similar to variables, but their values cannot be changed. They are defined using the `define()` function.
```bash
<?php
    define("PI", 3.14);
    echo "The value of PI is " . PI;
?>
```

### PHP Operators
Operators are used to perform operations on variables and values. PHP supports arithmetic, comparison, logical, and assignment operators.
```bash
<?php
    $x = 10;
    $y = 5;

    $sum = $x + $y;
    $isGreater = ($x > $y);
    $logicalAnd = ($x > 0) && ($y < 10);
?>
```
### PHP If & Else & Elseif
Conditional statements are used to perform different actions based on different conditions.
```bash
<?php
    $age = 25;

    if ($age < 18) {
        echo "You are a minor.";
    } elseif ($age >= 18 && $age < 65) {
        echo "You are an adult.";
    } else {
        echo "You are a senior.";
    }
?>
```
### PHP Functions
Functions are blocks of reusable code. They are defined using the function keyword.
```bash
<?php
    function greet($name) {
        return "Hello, $name!";
    }

    $message = greet("John");
    echo $message;
?>
```
### PHP Arrays
Arrays are used to store multiple values in a single variable. They can be indexed or associative.

`Indexed` arrays use numeric indices, starting from 0 and created using square brackets.
```bash
<?php
    $indexedArray = [1, 2, 3, 4, 5];
?>
```
`Associative` arrays use named keys to associate values, and use key-value pairs.
```bash
<?php
    $associativeArray = ["name" => "John", "age" => 25];
?>
```
### PHP Loop
Loops are used to execute a block of code multiple times. PHP supports for, while, do-while, and foreach loops.

The `for` loop is used when a specific number of iterations is known.
```bash
<?php
    for ($i = 0; $i < 5; $i++) {
        echo "Iteration $i <br>";
    }
?>
```
The `while` loop continues iterating as long as the specified condition is true.
```bash
<?php
    $counter = 0;
    while ($counter < 3) {
        echo "Counter: $counter <br>";
        $counter++;
    }
?>
```
The `do-while` loop is executed once before the condition is checked. If the condition is true, the loop will continue to execute.
```bash
<?php
    $number = 0;
    do {
        echo "Number: $number <br>";
        $number++;
    } while ($number < 3);
?>
```

The `foreach` loop is particularly useful for iterating over elements in an array or other iterable objects.
```bash
<?php
    $colors = ["Red", "Green", "Blue"];
    foreach ($colors as $color) {
        echo "Color: $color <br>";
    }
?>
```
