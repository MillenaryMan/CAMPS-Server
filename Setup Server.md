# Setup Server
## 1. Create the Server.cfg File
To setup the server, you need to create the Server.cfg file with the specified content in the root/CAMPS-Server/Build/ folder.

Copy the following command and paste it into your terminal, then press Enter:

```bash
cat << EOF > /root/CAMPS-Server/Build/Server.cfg
ServerID=0
ServerKey=0
ServerName=My Server
ServerIP=127.0.0.1
ServerPort=7777
ServerMaxCCU=20
ServerMode=SCA
EOF
```
This command creates the Server.cfg file in the root/CAMPS-Server/Build/ folder.

## 2. Setup Server Configurations
You can then proceed with setting up your server. Below are the configuration parameters in the Server.cfg file:

- ServerID: Unique identifier for the server.
- ServerKey: Key for server authentication.
- ServerName: Name of the server.
- ServerIP: IP address of the server.
- ServerPort: Port number for server communication.
- ServerMaxCCU: Maximum concurrent users allowed on the server.
- ServerMode: Server mode (e.g., SCA, TDM, DM, EXT, CR).
  
> [!IMPORTANT]
> Each server must pass the authentication process before it will be listed in the player's lobby.
> Servers with failed authentication will be ignored or represented as unwanted.
> To become a partner and receive a ServerID and ServerKey, please contact us via [Discord](https://discord.gg/xRbkcayDQS) or email us at millenaryinfo@gmail.com.

If you want to make your server always run on startup, follow the instructions at [Automize Server](https://github.com/MillenaryMan/CAMPS-Server/blob/main/Automatic%20Startup.md)
