# ASP9

Here we are again: A new version of .NET has been released, and so I am creating a new repo with source code, commands and links, so that you can create ASP.NET container images of 224 MB (default), 117 MB (chiseled), or 44 MB (chiseled and trimmed). Choose whichever you prefer :-) 

```
dotnet publish /p:PublishProfile=DefaultContainer

dotnet publish -p:PublishProfile=DefaultContainer -p:ContainerFamily=noble-chiseled

dotnet publish -p:PublishProfile=DefaultContainer -p:ContainerFamily=noble-chiseled -p:PublishTrimmed=true --sc
```

Sources: 

[dotnet-docker repo](https://github.com/dotnet/dotnet-docker/tree/main/samples/aspnetapp)

[Rich Lander's container-workshop](https://github.com/richlander/container-workshop/)

[my blog post](https://blog.pdebruin.org/aspnet-chisel-trim/)

[my asp9 images at docker hub](https://hub.docker.com/r/pdebruin/asp9/tags)