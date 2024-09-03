Installing SteamCMD
SteamCMD is a command-line version of the Steam client. 
To install it on Ubuntu follow next steps, to install it on other OS follow official guide: https://developer.valvesoftware.com/wiki/SteamCMD

1. Downloading SteamCMD on Ubuntu.
```
sudo add-apt-repository multiverse; sudo dpkg --add-architecture i386; sudo apt update
sudo apt install steamcmd
```
2. Install the dependencies required to run SteamCMD.
```
sudo apt-get install lib32gcc-s1
```
3: Run SteamCMD and login to your Steam client that owns the CAMPS game:
```bash
steamcmd
```
4: Login to your Steam client that owns the CAMPS game.
```bash
login <username>
```
5: Download/update CAMPS Server.
```bash
app_update 2948910
```
That's it, CAMPS server has been installed.

> [!TIP]
Run game as a PM2 process with auto start on startup.
PM2 is a production process manager for Node.js applications, but it can also manage any other processes, making it useful for running and monitoring applications such as CAMPS game servers.

1. Install PM2
```
sudo apt-get install nodejs npm
sudo npm install -g pm2
```
2. Start CAMPS Server with PM2
```
pm2 start /root/.local/share/Steam/steamapps/common/CAMPS-Server/CAMPS_LinuxServer_Core.x86_64 --name CAMPS-Server
```
3. Add PM2 to Startup
```
pm2 startup
pm2 save
```
