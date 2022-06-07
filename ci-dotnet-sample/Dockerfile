FROM mcr.microsoft.com/dotnet/aspnet:6.0 AS base
WORKDIR /app
EXPOSE 80
EXPOSE 443

FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build
WORKDIR /src
COPY ["ci-dotnet-sample/ci-dotnet-sample.csproj", "ci-dotnet-sample/"]
RUN dotnet restore "ci-dotnet-sample/ci-dotnet-sample.csproj"
COPY . .
WORKDIR "/src/ci-dotnet-sample"
RUN dotnet build "ci-dotnet-sample.csproj" -c Release -o /app/build

FROM build AS publish
RUN dotnet publish "ci-dotnet-sample.csproj" -c Release -o /app/publish

FROM base AS final
WORKDIR /app
COPY --from=publish /app/publish .
ENTRYPOINT ["dotnet", "ci-dotnet-sample.dll"]
