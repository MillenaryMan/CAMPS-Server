# Installing CAMPS server.

## 1. Install Git.
Update the package index and install Git using your package manager. On Ubuntu, you can use the following commands:
```sql
sudo apt update
sudo apt install git
sudo apt install git-lfs
```
If you're using a different Linux distribution, replace apt with your distribution's package manager, such as yum for CentOS or zypper for openSUSE.

## 2. Clone CAMPS server repository.
Clone CAMPS Server Azure repository using the git clone command:
```bash
git clone https://MillenaryGames@dev.azure.com/MillenaryGames/CAMPS-Server/_git/CAMPS-Server
```
This command will clone the repository to the current directory (/root/CAMPS-Server/).

## 3. Authenticate.
> [!NOTE]
> Git will prompt you to enter username and password or access token.
> 
> Username: campsserver@hotmail.com
> 
> Token: zlk5dhpb64xitrlggawwtivrrorvqkqwiwtahh7bq4v2ly5qsmaa (Will expire 1 January 2025)

## 4. Make Executables.
- Navigate to the Build derictory: 
```bash
cd /root/CAMPS-Server/Build/
```
- Make CAMPS.x86_64 executable:
```bash
chmod +x CAMPS.x86_64
```
- Make Start_Server.sh executable:
```bash
chmod +x Start_Server.sh
```

## That's it! :+1: You have successfully installed CAMPS server on your server machine.
You can now [Setup CAMPS Server](https://github.com/MillenaryMan/CAMPS-Server/blob/main/Setup%20Server.md).

> [!NOTE]
> After the cloning process completes, you can verify that your repository has been cloned successfully by listing the contents of the /root/CAMPS/ directory:
```bash
ls /root/CAMPS-Server/
```
You should see the files and directories from this Git repository.

