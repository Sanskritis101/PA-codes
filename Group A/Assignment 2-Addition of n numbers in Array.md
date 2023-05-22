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



