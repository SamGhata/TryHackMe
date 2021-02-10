Script package written for the TryHackMe Room Looking Glass. 

# Usage

Create local copies of the three files:<br>
LG-primer<br>
LG-cipher<br>
LG-reboot<br>

Make all three files executable with `chmod +x LG-*`<br>

Open a terminal to catch the reverse shell as:<br>
`nc -nlvp 8008`

In another terminal, run the primer script as:<br>
./LG-primer TARGET_IP LOCAL_IP<br>

The script will automatically:<br>
* find the correct port for the Dropbear SSH service
* connect to the service and solve the cipher challenge
* collect login credentials for jabberwock on SSH port 22
* login and alter the twasBrillig.sh for a reverse shell
* execute `sudo reboot` to send the shell to your waiting listener

