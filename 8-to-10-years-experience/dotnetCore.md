1. What is the difference between .Net & .NetCore?
2. How the `ConfigureService` & `Configure` method is getting used?
3. Why ConfigureService & Configure methods are used.
4. How to use **exception handing** in aspnetcore?\
Answer:- Exception handling in AspNetCore can be done in 3 places based on requirement.\
    * Code level(Using try/catch)\
    * Controller level (using action filter `IExceptionFilter`)
        - Don't have before and after events.
        - Implement OnException or OnExceptionAsync.
        - Handle unhandled exceptions that occur in Razor Page or controller creation, model binding, action filters, or action methods.
        - Do not catch exceptions that occur in resource filters, result filters, or MVC result execution.
    * Globally(using `UseExceptionHandler` middle ware)\

    > **NOTE:-** When to use what?\
 Concerned about errors in AspNet Framework level **useMiddleWare**.\
 Concerned about errors in MyCode **UseFilter**.

5. What are these files `*.deps.json` & `*.runtimeconfig.json`?
6. What is the benefit of using `[ApiController]` attribute?