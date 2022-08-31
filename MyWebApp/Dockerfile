FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build-env
WORKDIR /app

COPY *.csproj .
RUN dotnet restore

COPY Program.cs .
RUN dotnet build