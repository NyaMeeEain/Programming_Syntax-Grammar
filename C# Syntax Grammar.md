```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Hello
{
    class Program
    {
        static void Main(string[] args)
        {
            string one = "abc";
            string two = "123";
            string combined = one + two;
            Console.WriteLine(combined);
            Console.ReadKey();
        }
    }
}
```
### Boolean 
```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
namespace DemoApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Boolean status = true;
            Console.Write(status);

            Console.ReadKey();
        }
    }
}
```

### Integer
```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Integer
{
    class Program
    {
        static void Main(string[] args)
        {
            Int32 num = 30;
            Console.Write(num);
            Console.ReadKey();
        }
    }
}

```

### Double Boolean
```

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Double
{
    class Program
    {
        static void Main(string[] args)
        {
            double num = 30.33;
            Console.Write(num);
            Console.ReadKey();
        }
    }
}

```
### Variables
```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
namespace DemoApplication
{
    class Program
{
    static void Main()
    {
        var name = "Steve"; // use your name here
        Console.WriteLine($"Hello {name}!");
    }
}
}
```
### For Loops
```

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
public class Program
{
    public static void Main()
    {
        for (int i = 0; i < 10; i++)
        {
            Console.WriteLine(i);
        }
    }
}
```

# Decisions

### If 

```

using System;

class Program
{
    static void Main()
    {
        Greet(""); 
    }

    static void Greet(string name)
    {
        if (String.IsNullOrEmpty(name)) return;

        Console.WriteLine($"Hello, {name}!");
    }

```

### Or Else
```
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("What is the capital of Myanmar ?");
        var answer = "your answer here"; 
        if (answer.ToLower() == "Yangon")
        {
            Console.WriteLine("It is true!!!");
        }
        else
        {
            Console.WriteLine("Sorry, that's not the right answer.");
        }
    }
}
```

```
using System;

namespace Conditional
{
	class Program
	{
		public static void Main(string[] args)
		{
			int number = 10;

			if (number < 5)
			{
				Console.WriteLine("{0} is less than 5", number);
			}
			else if (number > 5)
			{
				Console.WriteLine("{0} is greater than 5", number);
			}
			else
			{
				Console.WriteLine("{0} is equal to 5");
			}
		}
	}
}
```
### C# Class
```
class Car 
{
  string color = "red";
  int maxSpeed = 200;

  static void Main(string[] args)
  {
    Car myObj = new Car();
    Console.WriteLine(myObj.color);
    Console.WriteLine(myObj.maxSpeed);
  }
}
```

```
class Car 
{
  string color;
  int maxSpeed;

  static void Main(string[] args)
  {
    Car myObj = new Car();
    myObj.color = "red";
    myObj.maxSpeed = 200;
    Console.WriteLine(myObj.color);
    Console.WriteLine(myObj.maxSpeed);
  }
}
```
