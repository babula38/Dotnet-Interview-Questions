1. What is the output of below program?
```csharp

using System;

namespace Test
{
    class Program
    {
        static void Main(string[] args)
        {
            Base obj = new Derive();
            obj.F1();
            obj.F2();
            obj.F3();
            Console.WriteLine("Hello World!");
        }
    }


    public class Base
    {
        public void F1() { Console.WriteLine("Base F1"); }
        public virtual void F2() { Console.WriteLine("Base F2"); }
        public virtual void F3() { Console.WriteLine("Base F3"); }
    }

    public class Derive : Base
    {
        new public void F1()
        {
            Console.WriteLine("Derive F1");
        }

        public override void F2()
        {
            Console.WriteLine("Derive F2");
        }

        public new void F3()
        {
            Console.WriteLine("Derive F3");
        }
    }
}


```
