# Hacker vs. Hacker TryHackMe room 
Difficulty: Easy

 **Prompt:**
The server of this recruitment company appears to have been hacked, and the hacker has defeated all attempts by the admins to fix the machine. They can't shut it down (they'd lose SEO!) so maybe you can help?

Run a nmap scan using the -sV flag (services and versions).

`nmap -sV http://10.10.95.41/`

Current Goal: find services that either have a version that is out of date and can be exploited or anything misconfigured.

Results: 

<img src="images/A1.png" width=750>

We can see that port 80 (HTTP) and port 22 (SSH) are open. From here we can attempt Enumuration of the HTTP website. 

I will be using Dirb in order to enumurate directories on this HTTP website 

