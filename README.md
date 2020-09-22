<div align="center">

## Absolute Recursive factorial function


</div>

### Description

Recursive factorial function a recursive function is a function that will call itself

it is probably the most difficult type of function designing

but when you get use to it, you'll find it VERY USEFULL the c++ version of this function is also available write here.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Arjang](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/arjang.md)
**Level**          |Intermediate
**User Rating**    |3.0 (6 globes from 2 users)
**Compatibility**  |C
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/arjang-absolute-recursive-factorial-function__3-752/archive/master.zip)

### API Declarations

stdio.h


### Source Code

```
/* Recursive factorial function programmed by Arjang
For more info email me arjang7@hotmail.com
a recursive function is a function that will call itself
it is probably the most difficult type of function designing
but when you get use to it, you'll find it VERY USEFULL
the c++ version of this function is also available write here.
*/
//inserting header file
#include<stdio.h>
//declaring function
int factorial(int);
void main(void)
{
	int number, result;
	printf("Please Enter A number to get it's factorial: ");
	//getting our target number
	scanf("%d", &number);
	//calling the function
	result = factorial(number + 1);
	//printing out results
	printf("\nThe factorial is : %d", result);
	printf("\n\n\n\n\n\n");
}
int factorial(int victim)
{
	if(victim>1)
	{
		victim = victim - 1;
		/*this is the whole point where you actually call the same function
		which you are into, it is called a recursive function. */
		victim = victim * factorial(victim);
	}
	return victim;
}
```

