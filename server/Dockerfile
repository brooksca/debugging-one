# Use the official .NET Core SDK as a parent image
FROM mcr.microsoft.com/dotnet/sdk:8.0
WORKDIR /app

# Copy the project file and restore any dependencies (use .csproj for the project name)
COPY src/*.csproj ./
RUN dotnet restore

# Copy the rest of the application code
COPY src/* ./

# Expose the port your application will run on
EXPOSE 8080

# Start the application
ENTRYPOINT ["dotnet", "watch"]