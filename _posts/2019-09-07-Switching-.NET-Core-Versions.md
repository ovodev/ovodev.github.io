---
layout: post
title: Switching .NET Core Versions
---

- Unlike .NET Framework, different .NET Core versions could be installed side by side each others.

- .NET Core SDKs are installed in
```
C:\Program Files\dotnet\sdk
```


-  To view the current active .NET Core version
```
dotnet --version
```


- To view all installed SDKs
```
dotnet --info
```

- To change .NET Core version
```
dotnet new globaljson --sdk-version 2.2.300
```

Documentation:
\
https://docs.microsoft.com/en-us/dotnet/core/versions/selection
