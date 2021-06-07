# Blazor_DisposeAsync_Sample

Test project to reproduce the following:  
.NET 6 (https://github.com/dotnet/aspnetcore/pull/32901) breaks the JS invocation from the `IAsyncDisposable.DisposeAsync()` method.

## Summary

.NET 5: 
Run the NET5\NET5\NET5.csproj project;
Refresh a browser page;
Wait for a while;
There is no an error in log.

.NET 6:
Run the NET6\NET6\NET6.csproj project;
Refresh a browser page;
The unhandled JSDisconnectedException exception is logged.
