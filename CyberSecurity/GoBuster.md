<h1>GoBuster</h1>

<b>GoBuster</b> is a tool used to brute-force URIs (directories and files), DNS subdomains and virtual host names.
For this machine, we will focus on using it to brute-force directories.

<b>gobuster dir -u http://<ip>:3333 -w word list location </b>

/usr/share/wordlists.
  
  
GoBuster flag
Description
-e
Print the full URLs in your console
-u
The target URL
-w
Path to your wordlist
-U and -P
Username and Password for Basic Auth
-p <x>
Proxy to use for requests
-c <http cookies>
Specify a cookie for simulating your auth
