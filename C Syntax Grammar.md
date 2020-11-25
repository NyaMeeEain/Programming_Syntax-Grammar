### Making Decisions
```
int main()
{
   int mark = 100;
   if (mark >= 39)           
   {
      printf("You Pass!\n"); 
   }
   else
   {
      printf("You Fail!\n");
   }
 
   return 0;
}
```

```
#include <stdio.h>
int main()
{
    int testInteger;
    printf("Enter an integer: ");
    scanf("%d", &testInteger);  
    printf("Number = %d",testInteger);
    return 0;
}
```
```
#include <stdio.h>
int main()
{
    char chr;
    printf("Enter a character: ");
    scanf("%c",&chr);     
    printf("You entered %c.", chr);  
    return 0;
}
```

### variable
```
int main() {
int x, y;
float salary = 13.48;
char letter = 'K';
x = 25;
y = 34;
int z = x+y;
printf("%d \n", z);
printf("%f \n", salary);
printf("%c \n", letter);
return 0;}
```
### Array
```

#include<stdio.h>
int main{
int a[7] = {1,2,3,4,5,6,7};
int i;
for(i=0;i<7;i++){
printf(“%d\n”,a[i]);
}
return 0;
}
```
