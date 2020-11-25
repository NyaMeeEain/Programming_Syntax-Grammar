#  C# Object-Oriented Programming.

### Direct Call The Class Name into Main Function
```
using System;
using System.Windows;
using System.Windows.Forms;


namespace Classs_Tut
{
    class Program
    {
        static void Main(string[] args)
        {

            Console.WriteLine("Hello");
            Honda.Show_Me();
            BMW.BME_Class();
        }
    }
    class Honda {
        public static void Show_Me()
        {
            MessageBox.Show("Hi");
        }
    }
    class BMW { 
        public static void BME_Class()
        {
            Console.WriteLine("Hello, This is BMW Class");
        }
    }
}

```

### Instance object c# Calling Object into Main Classs
```

using System;
using System.Windows;
using System.Windows.Forms;


namespace Classs_Tut
{
    class Program
    {
        static void Main(string[] args)
        {

            new Test().Test_Object();
            new BMW(). BMW_Object();
        }
    }
    class Test {
        public  void Test_Object()
        {
            MessageBox.Show("Hello");
        }
    }
    class BMW { 
        public  void BMW_Object()
        {
            Console.WriteLine("Hello, This is BMW Class");
        }
    }
}

```

### Storing The Class in to Memory 

```
using System;
using System.Windows;
using System.Windows.Forms;


namespace Classs_Tut
{
    class Program
    {
        static void Main(string[] args)
        {
            var memory = new Test();
            memory.Test_Object();
        }
    }
    class Test {
        public  void Test_Object()
        {
            MessageBox.Show("Hello");
        }
    }
    class BMW { 
        public  void BMW_Object()
        {
            Console.WriteLine("Hello, This is BMW Class");
        }
    }
}

```

### Undeclared Variable 
```
using System;




namespace Classs_Tut
{
    class Program
    {
        static void Main(string[] args)
        {
            var memory = new car(); // All the Data from Name will be stored into memory variable
            memory.name = "BMW";
            memory.name = "Ford";
            memory.name = "Tesla";
            memory.name = "Volkswagen";
            memory.name = "Chevrolet ";
            memory.name = "Toyota";
            System.Console.WriteLine(memory.name);
            System.Console.WriteLine(memory.name);
            System.Console.WriteLine(memory.name); //Calling The Name from Main Function in order to execute
        }
    }

    class car
    {
        public string name; //undeclared variable 


    }
}

```
### Calling Method Into The main Function
```
using System;




namespace Classs_Tut
{
    class Methods //Methods Class
    {
        static void Main(string[] Methods) //Define Methods Class into Main Function
        {
            Methods_Will_Be_Here(); // Calling Method Into The main Function
        }
        static void Methods_Will_Be_Here()
        {
            Console.WriteLine("Hello This is Methods");
        }
    }

   
}

```

### Array In C#
```
using System;




namespace Classs_Tut
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] ary = { "Thiri Soe ", "Marlene Lwin", "Aeindra", "Sanda","Kaymar Khaing" ,"NIlar"};
            Console.WriteLine(ary[3]);

        }


    }
}
```
