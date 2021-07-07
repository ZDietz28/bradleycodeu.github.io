---
layout: project
category: textgames
title: Caesar Cipher
permalink: /apcsp/textgames/caesarCipher/
---

Caesar Cipher (or Caesar Shift) is one of the simplest encryption techniques. It is a type of substitution in which each letter is replaced by a letter a set number away. For example, with a left shift of 3, D -> A, E -> B, and so on. Decrypt by shifting the same number in the opposite direction. The method is named after Julius Caesar.

![Caesar shift example](/apcsp/textgames/Caesar_cipher_left_shift_of_3.png)

Here is the encryption algorithm you will use:
```
def caesarEncrypt(myString,myNumber):
  result = ""
  # loop thru the string saving each letter in the varable each
  for each in myString:
    # convert each letter to a number
    letterNumber = ord(each)
    # shift the letter number by adding mynumber
    shiftedNumber = letterNumber + myNumber
    # convert the number back to character and string
    result += str(chr(shiftedNumber))
  return result
```

Based on the above encryption algorithm you should be able to create a separate caesarDecrypt function. It requires two arguments: myString,myNumber. It returns a string that has been shifted -myNumber places.

Define a function named randomSecretCodeWords that requires no arguments. Create three arrays with 10 words in each array. You might create an array of 10 fruits, another array of 10 colors, and an array of 10 cities. Concatenate the arrays just like you would concatenate strings: combinedList = list1 + list2 + list3. Use the [random choice function](https://www.w3schools.com/python/ref_random_choice.asp) to randomly select one word from the combined list. Concatenate THREE random words and return the result. For example, testing this function out five times could give the following result...
```
"redlimeMiami"
"graybananabanana"
"NYCDaytongrape"
"yellowLAgray"
"neonParisblack"
```

Define a function named validInt that requires one argument: userInput. Try to convert userInput to an int. If it works, return True. If there is an exception, return False.

Here is the pseudocode for the main function:
```
def main():
  # call randomSecretCodeWords() and save what is returned in secretString
  # generate a random int between 1 and 20 and save it in secretNumber
  # call caesarEncrypt with arguments secretString and secretNumber
  # then save what it returns in a variable named gibberish
  # output The gibberish message is: and concatenate the gibberish variable
  # create a forever loop
    # output Shift by how much? Type 1-20
    # collect the user input
    # if the user input is valid
      # convert the user input to an int
      # call caesarDecrypt with agruments gibberish and user input
      # then save what it returns in a variable named newText
      # output the new decrypted text
      # if the userInput is the secretNumber
        # break out of the loop
```
