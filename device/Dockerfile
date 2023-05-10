# Use the official Microsoft .NET 5.0 SDK image as the base image
FROM mcr.microsoft.com/dotnet/aspnet:5.0

# Expose the necessary ports for Azure Device Streams (2222) and HTTPS (443)
EXPOSE 2222
EXPOSE 443

# Copy everything
COPY . /App

WORKDIR /App

ENTRYPOINT ["dotnet", "run", "--project", "device.csproj", "\"HostName=Balajitesthub.azure-devices.net;DeviceId=iottestdev1;SharedAccessKey=hw0BJR/a0oyhHk+hZsC3/k62bPITIJLxUPRMzhU2D7k=\"","localhost", "22"]
