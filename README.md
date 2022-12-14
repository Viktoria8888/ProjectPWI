## Polynomials
### To make the program work correctly make sure to do:
```
$pip install matplotlib
```
The program takes the list of coefficients as an argument and performs different functions on it. In particular,
 1) Converts an expanded polynomial to a factored polynomial.

 2) Generates a graph of a polynomial in a specified range.

 3) Determines the maximum and minimum global values.

 4) Returns all the polynomial roots in expanded form within a given range and with a given approximation.

 5) A function that parses a string, given as a parameter, as a polynomial in one of the representations and returns a pair of one of three forms:
 - ("współczynnikowa", lista),
 - ("pierwiastkowa", lista), or
 - ("błąd parsowania", [])
 where lista represents the given polynomial in the given way.
 The string given as a parameter should be in the form of space-separated monomials in descending order of the degree of the monomial, or parentheses raised to a certain power separated by a space. 
 The ^ character should be used as a power symbol.
 For example:
 - correct input: '(x-7) x^3 (x+2)^3 (x+6)^2', '2x^6 -x^4 +13x^3 +278x^2 +9'
 - incorrect input: '2x-3', 'x^7 -(x+2)', '(x-1)(x+9)'
 For monomials of the form x raised to a certain power, the function returns the factored representation. 
 For example, for input 'x^3' the function returns ("współczynnikowa", [0, 0, 0]) rather than ("pierwiastkowa", [1, 0, 0, 0]).
