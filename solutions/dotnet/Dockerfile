# https://hub.docker.com/r/microsoft/dotnet/
FROM microsoft/dotnet:2.2-sdk

COPY ./dotnet-example /app
WORKDIR /app

RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]

EXPOSE 5000/tcp

CMD dotnet run --urls http://0.0.0.0:5000
