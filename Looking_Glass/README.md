Bash script written for the TryHackMe Room Looking Glass. The first task is to discover which of the 5,000 open SSH ports will complete a connection. This script finds the correct port.

usage:<br>
./ssh-search 10.10.154.209

example result:<br>
Testing..............<br>
Connect to the real SSH service using:<br>
ssh 10.10.154.209 -p 13484%  <br>

Note - the trailing "%  " is an artifact I can not find the source of or correct at this time.
