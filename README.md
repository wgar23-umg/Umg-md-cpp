# Umg-md-cpp

# Funcionamiento de Sentencia *`if-else`* en C++

Una instrucción if-else controla la bifurcación condicional. Las instrucciones de `if-branch` se ejecutan solo si se `condition` evalúa como un valor distinto de cero (o `true`). Si el valor de `condition` es distinto de cero, se ejecuta la siguiente instrucción y se omite la instrucción que sigue a la instrucción `else` opcional. De lo contrario, se omite la siguiente instrucción y, si hay una instrucción `else`, la instrucción siguiente `else` se ejecuta.

***

## Ejemplo

    #include <iostream>

    int main()
    {
        std::cout << "Enter an integer: ";
        int x {};
        std::cin >> x;

        if (x == 0)
            std::cout << "The value is zero\n";

        return 0;
    }

El ejemplo anterior valida si el valor ingresado es un valor entero. Si es 0, no lo indicara de lo contrario, no hará nada.

***

# Funcionamiento de sentencia *`Switch`* en C++

Permite seleccionar código entre multiples secciones, en función del valor de una expresión entera.

Las expresiones que evalúan a tipos de punto flotante, cadenas y la mayoría de los otros tipos no integrales no pueden ser usadas aquí.

***

## Sintaxis

    #include <iostream>

    void printDigitName(int x)
    {
        switch (x) // x is evaluated to produce value 2
        {
        case 1:
            std::cout << "One";
            return;
        case 2: // which matches the case statement here
            std::cout << "Two"; // so execution starts here
            return; // and then we return to the caller
        case 3:
            std::cout << "Three";
            return;
        default:
            std::cout << "Unknown";
            return;
        }
    }

    int main()
    {
        printDigitName(2);
        std::cout << '\n';

        return 0;
    }

***

# Referencias

### Sentencias *`If-Else`* y *`Switch`*

**[Microsoft Learn C++ - www.learn.microsoft.com](https://learn.microsoft.com/en-us/cpp/?view=msvc-170)**

**[Learncpp - www.learncpp.com](https://www.learncpp.com/)**