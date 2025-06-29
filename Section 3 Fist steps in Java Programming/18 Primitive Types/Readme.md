## PRIMITIVE TYPES

1. When will get an overflow? When will get an error

    When you are using __expression__ that are not a simple __literal value__ => get an overflow

        Ex: int minValue = Integer.MIN_VALUE - 1

        Ex: int minValue = -2147483648 - 1
    

     When you are using  a simple __literal value__ => get an error

        Ex: int minValue = -2147483649 (-2147483649 is an int __literal value__)

    Note: In Java, a __simple literal value__ refers to a fixed, constant value written directly in the source code. It is not a variable, expression, or computed value — it’s just a raw value

2. What does an underscore mean in a numeric literal?

    Java provided an alternative way to improve readability, the underscore, you can't use an underscore at the start or end of the numeric literal.

        Ex: int myMaxVal = 2_147_483_647;
