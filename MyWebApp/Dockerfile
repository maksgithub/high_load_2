# FROM mcr.microsoft.com/dotnet/aspnet:6.0 AS base
# WORKDIR /app

FROM alpine
RUN mkdir -p /tmp/dir && touch /tmp/dir/file1 /tmp//dir/file2
RUN file="$(ls -1 /tmp/dir)" && echo $file
RUN echo $(ls -1 /tmp/dir)
RUN echo "Hello StackOverflow!"
# RUN dotnet build "ConversaoPeso.Web.csproj" -c Release -o /app/build