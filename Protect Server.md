# 1. Monitor Network Traffic
If you prefer a graphical user interface, you can use the Gnome System Monitor to monitor bandwidth usage
To install Gnome System Monitor, open a terminal and run:

```bash
sudo apt-get install gnome-system-monitor
```
Once installed, you can typically launch these tools from the terminal by typing their names or find them in your system's application menu. 

# 2. Open/Close ports (Configure Firewall Rules)
To open or close a port on Ubuntu, you can use the Uncomplicated Firewall (UFW) which is a frontend for managing firewall rules in Ubuntu.
* Install UFW if not already installed:
```sql
sudo apt update
sudo apt install ufw
```

* Open a Port:
To allow incoming traffic on a specific port, you can use the following command:
```bash
sudo ufw allow <port_number>
```
Replace <port_number> with the actual port number you want to open. For example, to open port 80 (HTTP), you would run:
```bash
sudo ufw allow 80
```

* Close a Port:
To deny incoming traffic on a specific port, you can use the following command:
```bash
sudo ufw deny <port_number>
```
Replace <port_number> with the actual port number you want to close. For example, to close port 80 (HTTP), you would run:
```bash
sudo ufw deny 80
```

* Reload UFW:
After making changes to UFW rules, it's a good practice to reload the firewall to apply the changes. You can do this by running:
```bash
sudo ufw reload
```

* Check Status:
To check the status of UFW and see the list of rules, you can use the following command:
```bash
sudo ufw status
```
This will display the current status of UFW and the list of rules, including the ports that are allowed or denied.

