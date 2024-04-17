1: Installing SteamCMD
SteamCMD is a command-line version of the Steam client. To install it, follow this official guide: https://developer.valvesoftware.com/wiki/SteamCMD

2: Add Steam path to global varibles.
```bash
export PATH=$PATH:/usr/games
```
3: For security reasons login as steam user instead of root user.
```bash
sudo -u steam -s
cd /home/steam
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

That's it, CAMPS server has been isntalled.
