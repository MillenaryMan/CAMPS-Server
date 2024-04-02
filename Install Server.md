# Installing CAMPS server.

## 1.Install Git.
Update the package index and install Git using your package manager. On Ubuntu, you can use the following commands:
```sql
sudo apt update
sudo apt install git
```
If you're using a different Linux distribution, replace apt with your distribution's package manager, such as yum for CentOS or zypper for openSUSE.

## 2.Clone CAMPS server repository.
Clone CAMPS Server repository using the git clone command:
```bash
git clone https://github.com/MillenaryMan/CAMPS-Server.git
```
This command will clone the repository to the current directory (/root/CAMPS-Server/).

## 3.Authenticate (If Required).
> [!NOTE]
> Git will prompt you to enter your username and password or access token.
> 
> To create you access token, follow those steps: [How to create personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

## 4.Verify the Cloning.
After the cloning process completes, you can verify that your repository has been cloned successfully by listing the contents of the /root/CAMPS/ directory:
```bash
ls /root/CAMPS-Server/
```
You should see the files and directories from this Git repository.

## That's it! You have successfully installed CAMPS server on your server machine. 
You can now [Setup CAMPS Server](https://github.com/MillenaryMan/CAMPS-Server/blob/main/Setup%20Server.md).
