LED Blinking

**Code:**

```C
#include <xc.h>
#include <stdio.h>
#include <stdlib.h>
#include <pic18f4550.h>
void todelay(void)
{
T0CON = 0x08 ;
TMR0H = 0x77 ;
TMR0L = 0X00 ;

T0CONbits.TMR0ON = 1 ;
while(INTCONbits.TMR0IF==0);
T0CONbits.TMR0ON = 0 ;
INTCONbits.TMR0IF = 0 ;
}
void main(void)
{
TRISD = 0 ;
while(1)
{
PORTD = 0xAA ;
todelay();
PORTD = 0x00 ;
todelay();
}
```

**Output:**

![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/360d67e0-7c67-4b18-89e6-3316e2cb7b99)
