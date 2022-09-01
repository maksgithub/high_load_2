FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build-env
WORKDIR /app
EXPOSE 5042

COPY *.* .
RUN dotnet restore

COPY Program.cs .
RUN dotnet build "MyWebApp.csproj" -c Release -o ./build

WORKDIR /app/build
ENTRYPOINT ["dotnet", "MyWebApp.dll"]