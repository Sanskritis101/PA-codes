Addition of n numbers in array

**Code:**
```
#include <stdio.h>
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
    TRISB = 0;
    TRISD = 0;
    for(int n = 0; n<=4; n++){
        PORTB = source[n];
        PORTD = dest[n];
        for(int a = 0; a<1000; a++) {
            for(int j = 0; j<500; j++) {
            }
        }
    }
return 0;
}
```

**Output:**

![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/cb27ed5b-6c53-40f0-865e-33b46ba38859)

![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/d293cd1b-a9af-4679-8b00-d1365d751ec7)

