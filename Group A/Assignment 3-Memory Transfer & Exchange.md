Assignment 3

Write an Embedded C program to transfer elements from one location to another for following:  
i) memory transfer ii) memory exchange

Code:
```C
#include <stdlib.h>
#include <xc.h>
#include <pic18f4550.h>

int main()
{
    int source[] = {0x01, 0x02, 0x03, 0x04, 0x05};
    int dest[] = {0x00, 0x00, 0x00, 0x00, 0x00};
    for(int i = 0; i<=4; i++) {
        dest[i] = source[i];
    }
    TRISD = 0;
    for(int n = 0; n<=4; n++){
        PORTD = dest[n];
        for(int a = 0; a<1000; a++)  {
            for(int j = 0; j<500; j++)   {
           }
        }
    }
    return 0;
}
```

**Output:**

![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/15f41143-e15c-4dc0-827d-0ac9beb159a9)
