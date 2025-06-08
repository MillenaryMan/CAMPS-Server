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

```
dotnet publish -c Release -r linux-x64 --self-contained false -f net8.0 -o ./publish
```
```
dotnet publish -c Release -r linux-x64 --self-contained true -f net8.0 -o ./publish
```
