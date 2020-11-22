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
