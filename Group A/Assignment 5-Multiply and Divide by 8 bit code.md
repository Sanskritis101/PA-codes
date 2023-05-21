Multiply and Divide by 8 bit code

**Code:**

```C
#include <xc.h>
#include <stdio.h>
#include <pic18f4550.h>
void main(void){
    int a,b,mul;
    a = 0x06;
    b = 0x03;
    mul = 0x00;
    mul = a*b;
    TRISD = 0;
    PORTD = mul;
    return;
}
```

**Output:**
  
  ![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/5671080c-6c87-4bd6-bd8f-04d8f5b7869e)
