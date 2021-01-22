Script written for the TryHackMe Room Looking Glass. 
The first task is to discover which of the 5,000 open SSH ports will complete a connection. 
This script narrows the range to six ports to test manually.

usage:
ssh-search 10.10.16.141

example result:
The real SSH service is on one of the remaing ports from 10048 to 10053.
Test them using:
ssh -o StrictHostKeyChecking=No 10.10.16.141 -p 10048
