---
layout: project
category: ch1introduction
title: Ch1 Integer Overflow Practice
---

Java primitive data types (with ones we will use in APCSA <mark>highlighted</mark>):

  - byte: Byte data type is an 8-bit signed two's complement integer.

  - Short: Short data type is a 16-bit signed two's complement integer.

  - <mark>int: Int data type is a 32-bit signed two's complement integer.</mark>

  - long: Long data type is a 64-bit signed two's complement integer.

  - float: Float data type is a single-precision 32-bit IEEE 754 floating point.

  - <mark>double: double data type is a double-precision 64-bit IEEE 754 floating point.</mark>

  - <mark>boolean: boolean data type represents one bit of information.</mark>

  - char: char data type is a single 16-bit Unicode character.

What is a 32-bit signed two's complement integer? The value of the left-most binary column (aka the most significant bit or MSB) is flipped to negative.

Here are some *simpler* examples:

```
3-bit signed two's complement columns = -4 2 1 (min -4 to max 3)

4-bit signed two's complement = -8 4 2 1 (min -8 to max 7)

6-bit signed two's complement = -32 16 8 4 2 1 (min -32 to max 31)

8-bit signed two's complement = -128 64 32 16 8 4 2 1 (min -128 to max 127)
```

8-bit signed two's complement columns:

|Binary value|Two's complement|Unsigned|
|--- |--- |--- |
|00000000|0|0|
|00000001|1|1|
|⋮|⋮|⋮|
|01111110|126|126|
|01111111|127|127|
|10000000|−128|128|
|10000001|−127|129|
|10000010|−126|130|
|⋮|⋮|⋮|
|11111110|−2|254|
|11111111|−1|255|


## Directions

  Run the [IntOverflowGenerator app](https://repl.it/@JustinRiley1/IntOverflowGenerator#Main.java), then copy and paste the Console Output into a text document. 

  Solve the problems in your text document.

  Turn in your text document.

<iframe height="600px" width="100%" src="https://repl.it/@JustinRiley1/IntOverflowGenerator?lite=true&outputonly=1" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>
