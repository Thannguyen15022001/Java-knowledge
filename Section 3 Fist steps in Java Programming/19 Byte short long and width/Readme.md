## byte, short, int , long


| __Data Type__  | __Width (in bits)__ | __Min value__ | __Max value__ |
|----------------|--------------------|---------------|---------------|
|   byte         |       8            | -128          | 127           |
|   short        |       16           | -32168        | 32767         |       
|   int          |       32           | -2147483648   | 2147483647    |
|   long         |       64           | -9223372036854775808 | 9223372036854775807 |


Note: In Java __numeric literal__ by default, is an __int__, a numeric literal that exceeds Integer.MAX_VALUE must use the 'L' suffix
    
    Ex: long defaultNumericLiteral = 100;   100 is numeric literal default (data type is int)
    
    Ex: long longNumericLiteral = 100L;    100L has data type is long
    
    Ex: long myValue = 2_147_483_647_1;    Error due to numeric literal default is int (must use 'L' suffix)

    Ex: long myNewLongValue = 10 + (myMinLongValue / 2);    No error due to right is expression

    Ex: long myNewLongValue = 10 + (9223372036854775807 / 2);   Error due to right is numeric literal
