Timer as Counter

**Code:**

```C
#include <xc.h>
#include<pic18f4550.h>
#include<stdlib.h>
void main(){
TRISD=0x00;
T0CON=0x48;
TMR0L=0x00;
while(1){
T0CONbits.TMR0ON=1;
do{
/*PORTD=TMR0L;*/
for(int i=0;i<500 ;i++){
for(int j=0;j<100;j++){}
}
}

while(INTCONbits.TMR0IF==0);
PORTD=0xFF;
for(int i=0;i<100 ;i++){for(int j=0;j<100;j++){}}
T0CONbits.TMR0ON=0;
INTCONbits.TMR0IF=0;
if(T0CONbits.TMR0ON==0){
PORTD=0x00;}
}
}
```

**Output:**

![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/ee3260e3-4220-4f07-9646-ea60b83ab3a1)

![image](https://github.com/Sanskritis101/PA-codes/assets/104347305/9f095fa9-297a-42b1-967b-dc4030ed8216)
