Addition of n numbers in array

**Code:**
```C
#include <stdlib.h>
#include <xc.h>
#include <pic18f4550.h>


void main()
{
int num[] = {0x0A, 0x02, 0x03, 0x04, 0x06};
int result = 0x00;
for(int i =0; i<5; i++)
{
result = result + num[i];
}
TRISD = 0;
PORTD = result;

return;
}
```

**Output:**

![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/cb27ed5b-6c53-40f0-865e-33b46ba38859)

![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/d293cd1b-a9af-4679-8b00-d1365d751ec7)

