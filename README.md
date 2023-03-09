# Number-binary-converter

A program and UI to convert an integer to binary code through a custom function.

Try it out here: https://madgrv.github.io/Number-binary-converter/

## Overview

This program was created to explore and recreate a function that converts an integer to binary code. The process for the conversion involves repeatedly dividing the number by 2, keeping track of the remainder at each step, until the number becomes 0. The remainders are then concatenated in reverse order to obtain the binary code. This process is also known as "division by 2" or "successive halving".

The custom function used in this program is as follows:

```javascript
function binaryConvert(n) {
    let string = "";
    let reverse = "";

    while (n > 0) {
        string += n % 2;
        n = Math.floor(n / 2);
    }

    for (let i = string.length - 1; i >= 0; i--) {
        reverse += string[i];
    }
    return reverse;
}```

## Usage

To use this program, enter an integer into the input box on the web page and the corresponding binary code will be displayed.

## Built With

- HTML
- CSS
- JavaScript

## Acknowledgments

This program was inspired by a desire to learn more about binary code and how it is created.

