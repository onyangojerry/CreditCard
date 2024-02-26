# Haskell Credit Card Validation README

This Haskell module provides a collection of functions for credit card number validation. It includes utility functions for list manipulation, digit extraction, and the implementation of the Luhn algorithm for validating credit card numbers.

## Features

- **Digit Manipulation**: Convert integers to a list of digits and vice versa.
- **List Utilities**: Custom functions to zip lists, prepend elements, and rotate lists.
- **Credit Card Validation**: Implements the Luhn algorithm to check the validity of credit card numbers.

## Installation

Ensure you have GHC (Glasgow Haskell Compiler) installed on your system. You can download GHC from [https://www.haskell.org/ghc/](https://www.haskell.org/ghc/).

## Usage

### Importing the Module

Save the provided code into a file named `CreditCardValidator.hs`. In your Haskell script or GHCi, import the module by adding:

```haskell
import CreditCardValidator
```

### Functions

- `myZip`: Takes two lists and returns a list of pairs.
- `consAll`: Takes a list of lists and an element, prepending the element to every list.
- `cycleK`: Rotates the elements in a list by a given amount.
- `toDigits`: Converts a positive integer to a list of digits.
- `toDigitsRev`: Converts a positive integer to a list of digits in reverse order.
- `doubleEveryOther`: Doubles every other number in a list, starting from the right.
- `sumDigits`: Sums all digits in a list of integers.
- `validate`: Takes an integer and returns `True` if it's a valid credit card number according to the Luhn algorithm, otherwise `False`.

### Example

To validate a credit card number:

```haskell
main :: IO ()
main = do
  let cardNumber = 1234567890123456
  print $ validate cardNumber
```

## Contributions

Contributions to improve the code or extend the functionality are welcome. Please follow the standard Haskell coding guidelines for your contributions.

## License

This project is open-sourced under the MIT License. See the LICENSE file for more details.

---
