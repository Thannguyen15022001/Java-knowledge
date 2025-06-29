## Assigning expressions to variables with data types that don't match

Case 1: The Java compiler does not attempt to evaluate the value, in a variable, when it's used in a calculation, so it doesn't know if the value fits, and throws an error

    Ex: byte myNewByteValue = (myMinByteValue / 2);

Case 2: If your calculation uses literal values, Java can figure out the end result at compile time, and whether it fits into the variable, and won't throw an error if it does.

    Ex: byte myNewByteValue = (-128 / 2);

Case 4: This statement works because the result is an int, and assigning it to an int variable is fine.

    Ex: int myTotal = (myMinIntValue / 2);

Case 5: This statement doesn't work, because the expression (myMinShortValue / 2) is an int, and an int can't be assigned to a short, because the compiler won't guess the result.

    Ex: int myNewShortValue = (myMinShortValue / 2);

Case 6: 

    Ex: long myNewLongValue = 10 + (myMaxLongValue / 2);    No error

    Ex: long myNewLongValue = 10 + (9223372036854775807 / 2);  error
