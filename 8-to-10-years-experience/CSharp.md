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
2. Why `IDisposable` is used?
3. What is `Finalizer` is used for?
4. How **GC** works in .net?
5. What is difference between .Net and .Net Core?
6. What is difference between **Manged v/s unmanaged memory** in .Net?
7. If program is developed in .net core in Windows then can we run the same program in Linux without changing anything?
8. .Net core deployment modes?
9. What 4 pillars of OOPS?
10. What is **extension methods** and when to use?