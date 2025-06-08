```
sudo apt update
sudo apt install -y dotnet-sdk-8.0
```


```
dotnet --version
```

```
sudo ufw allow 7777/udp
```

Run From PM2
```
pm2 start "dotnet CAMPS.Server.dll" --name CAMPS-Server
```

# Linux
```
dotnet publish GameServer.csproj -c Release -r linux-x64 --self-contained false -f net8.0 -o ./publish/linux
```
# Windows
```
dotnet publish GameServer.csproj -c Release -r win-x64 --self-contained false -f net8.0 -o ./publish/windows
```
# macOS (Intel)
```
dotnet publish GameServer.csproj -c Release -r osx-x64 --self-contained false -f net8.0 -o ./publish/macos-x64
```
# macOS (Apple Silicon)
```
dotnet publish GameServer.csproj -c Release -r osx-arm64 --self-contained false -f net8.0 -o ./publish/macos-arm64
```
