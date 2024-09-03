# Setup Server
## 1. Server.cfg File
Open Server.cfg file in the /root/.local/share/Steam/steamapps/common/CAMPS-Server/ folder.
```
sudo nano /root/.local/share/Steam/steamapps/common/CAMPS-Server/Server.cfg
```
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
> To become a partner and receive a ServerID and ServerKey, please contact us via [Discord](https://discord.gg/camps) or email us at millenaryinfo@gmail.com.
