# Updating Server Build with Git

## 1. Terminate the Current Server Process
Before updating the server build, it's essential to stop the current server process to prevent conflicts or unexpected behavior.
- Check if the CAMPS-Server process is running
```bash
pgrep -f "CAMPS.x86_64"
```
- If the process is running, kill it
```bash
sudo pkill -f "CAMPS.x86_64"
```

## 2. Navigate to the Server Build Directory
Navigate to the directory where your server build is located. Assuming your server build is located in the /root/CAMPS-Server/Build/ directory:
```bash
cd /root/CAMPS-Server/Build/
```

## 3. Pull the Latest Changes from the Git Repository
Next, pull the latest changes from the Git repository to update your server build. Use the git pull command:
```bash
git pull
```
This command fetches the latest changes from the remote repository and merges them into your local branch.

## 4. Restart the Server Process (if Necessary)
If the server process needs to be restarted to apply the updates, you can do so using the appropriate commands. For example, if your server is managed by a systemd service called camps_server, you can restart it using:
```bash
sudo systemctl restart camps_server
```

Summary of Commands:
```bash
# Terminate the Current Server Process
pgrep -f "CAMPS.x86_64"
sudo pkill -f "CAMPS.x86_64"
# Navigate to the Server Build Directory
cd /root/CAMPS-Server/Build/
# Pull the Latest Changes from the Git Repository
git pull
# Restart the Server Process (if Necessary)
sudo systemctl restart camps_server
```
