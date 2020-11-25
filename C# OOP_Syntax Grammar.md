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

### Calling Object into Main Classs
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
