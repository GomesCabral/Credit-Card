# Credit-Card
Credit Card Checker

The purpose of validateCred() is to return true when an array contains digits of a valid credit card number and false when it is invalid. This function should NOT mutate the values of the original array.

  rules: 1) Starting from the farthest digit to the right, AKA the check digit, iterate to the left.
          2) As you iterate to the left, every other digit is doubled (the check digit is not doubled). If the number is greater than 9 after doubling, subtract 9 from                its value.
          3) Sum up all the digits in the credit card number.
          4)If the sum modulo 10 is 0 (if the sum divided by 10 has a remainder of 0) then the number is valid, otherwise, it’s invalid.
          
The role of findInvalidCards() is to check through the nested array for which numbers are invalid, and return another nested array of invalid cards.

idInvalidCardCompanies() that has one parameter for a nested array of invalid numbers and returns an array of companies.
Currently, there 4 accepted companies which each have unique first digits. The following table shows which digit is unique to which company:
        First Digit	Company
        3	    Amex (American Express)
        4	    Visa
        5	    Mastercard
        6	    Discover
        
        
 If the number doesn’t start with any of the numbers listed, print out a message like: “Company not found”.

idInvalidCardCompanies() should return an array of companies that have mailed out cards with invalid numbers. This array should NOT contain duplicates, i.e. even if there are two invalid Visa cards, "Visa" should only appear once in the array.
