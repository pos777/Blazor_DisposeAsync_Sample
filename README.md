# Blazor_DisposeAsync_Sample

Test project to reproduce the following:  
.NET 6 (https://github.com/dotnet/aspnetcore/pull/32901) breaks the JS invocation from the `IAsyncDisposable.DisposeAsync()` method.

## Summary

.NET 5: 
Run the https://github.com/pos777/Blazor_DisposeAsync_Sample/blob/master/NET5/NET5.sln project;
Refresh a browser page;
Wait for a while;
There is no an error in log.

.NET 6:
Run the https://github.com/pos777/Blazor_DisposeAsync_Sample/blob/master/NET6/NET6.sln project;
Refresh a browser page;
The unhandled JSDisconnectedException exception is logged.
![image](https://user-images.githubusercontent.com/5260725/120996932-7315ee80-c78f-11eb-8034-8b895e0969c1.png)
