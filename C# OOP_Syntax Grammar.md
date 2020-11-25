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
