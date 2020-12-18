1. what is explicit implementing interface?
2. What is GC?
3. What is Finalize and disposable?
4. How to call a base class constructor from derive class?
5. What is anonymous methods? where we are using?
6. What is multicast delegate?
7. Difference between Async vs sync?
8. Can i use await keyword in catch and finally?
9. Difference between `IEnumrable` vs `IQueryable`?
10. In case of lazy loading which one should be use `IEnumrable` vs `IQueryable`?
11. What is difference between `First` & `FirstOrDefault` in LINQ?\
------Asp.net-----
12. Difference between **http module** vs **http handler**
13. What is data annotation?
14. What is **DI or (dependency injection)**?
15. What is AntiForgeryToken?\
-------WebApi------
16. When to use WebApi?
17. What are http verbs?ANS:- verb describe the action
18. What is Attribute routing?
19. What is CORS(cross origin resource sharing)?
20. What is JWT token vs bearer token?
21. How exception is hand is done in webapi?\
-------ADO.net------
22. Difference between connected vs disconnected architecture?
23. What is connection pooling?
24. What is **maxpoolsize & minPoolSIze**?
25. Difference between **data reader vs dataset**?
26. What is difference between **Copy vs clone** in dataset?\
-------SQL-----
27. what is the difference between truncate vs delete?
28. What is index, how many types of index is present in SQL Server?
29. What is CTE?
30. How to use CTE to delete duplicate records?
31. How to create a new table from existing table without copying the data?
32. What is locking?\
---------ReactJS----
33. What is **JSX** file?
34. What is different between **class component vs functional component**?
35. What is difference between **state vs prop**?
36. What is pure component?
37. What is higher order component?
38. What is setState?
39. Difference between **super vs super(props)**
40. What is replace state method in component?
41. what is map function in javascript?\
-------mphasis----------
42. will the following code work?
```csharp
    public class MyClass
    {
        public int F1()
        {
            try
            {
                // data inconsistency, think what will happen if it
                //return 1 from try and return 0 from finally then what it should return
            }
            catch (Exception e)
            {
                return 1;
            }
            finally
            {
                return 0;
            }
    }
```
43. will the following code work?

```csharp
        public int F2()
        {
            try
            {

            }
            catch (Exception e)
            {
                return 1;
            }
            catch (DivideByZeroException cc)
            {
                return 0;
            }
        }
```
44. will the following code work?
```csharp
    public class MyClassxxx
    {
        int i = 0;
        i="hello world";

    }
```
45. Output of the following program?
```csharp
public class A
{
    static int j = i;
    static int i = 1;
        
    public static void Main()
    {
        Console.WriteLine($"cccc {i}-----{j}");
    }
}
```
46. Can we avoid nested call to call containing class private `constructor`?
47. Sequence of filter execution in MVC?
48. How your handling exceptions in webapi?
49. Explain SOLID principle? 
50. How did you achieve `liskov substitution` in your project
-----------------other------------
51. when can you suggest someone to use EF and WHY?
52. what is the different between `IEnumerable vs IQueryable` when to use what?
53. Do you prefer `SQl or stored procedure`?
54. IF you will gave an option which one you will prefer EF or Ado.net and why?
55. What will be the execution result of the following query?
```csharp
delegate void SomeMethod();

static void Main(string[] args)
{
    List<SomeMethod> delList = new List<SomeMethod>();
    for (int i = 0; i < 10; i++)
    {
        delList.Add(delegate { Console.WriteLine(i); });
    }

    foreach (var del in delList)
    {
        del();
    }
}
```
56. what is the output of the below code?
```csharp
void F1()
{
    {int i=0;}
    int j=i+1;
    Console.WriteLine($"The number is {j}")
}
```
56. what is the output of the below code?\
    Hints:- string interning
```csharp
string hello = "hello";
string helloWorld = "hello world";
string helloWorld2 = "hello world";
string helloWorld3 = hello + " world";

Console.WriteLine(helloWorld == helloWorld2);
Console.WriteLine(object.ReferenceEquals(helloWorld, helloWorld2));
Console.WriteLine(object.ReferenceEquals(helloWorld, helloWorld3));
``` 
-----preqin----\
57. Write singleton class?
58. Where you configure your dependency in Aspnetcore?
59. How .netcore run on multi platform?        
60. How do you send status code to client from Aspnetcore web api?
61. Well AspNetCore web api only support `json & XML` by default, what we need to do if we need a custom format?\
62. Have you even take part in architect design decisions, can you explain such recent incident where you have suggested some thing?\
63. How do you handle security in your applications?\
64. In DI what is the difference between `AddTransient & AddScoped` life time?\
65. How you do Sql performance optimization?\
66. What is kestrel server in aspnetcore & why it is used?\
-----------mphasis--------\
67. What is async programming in .net core?\
68. Where you configure your routing in .net core?\
69. Given a scenario you need to connect 3 services to aggregate the result and send to the client how would you do that in .net?\
70. What is swagger?
71. SOLID?
72. Name a design pattern you have used and why?
