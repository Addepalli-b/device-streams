# Use the official Microsoft .NET 5.0 SDK image as the base image
FROM mcr.microsoft.com/dotnet/sdk:5.0

# Expose the necessary ports for Azure Device Streams (2222) and HTTPS (443)
EXPOSE 2222
EXPOSE 443

# Copy everything
COPY . /App

WORKDIR /App

ENTRYPOINT ["dotnet", "run", "--project", "device.csproj"]
