# WannaHack CTF
>This was the information provided 
```
 I made a binary calculator yay!

Challenge Link: http://ctf.copsiitbhu.co.in:21338/

NOTICE: Solving this challenge unlocks another challenge

```
so following the link took me to the page that looked something like that

![](https://github.com/Wizzy2323/WannaHackme/assets/159465554/5aa855ab-eff4-4387-8d84-04ee43104309)

So first doing all the starting rituals like inspecting and looking at page source and the cookies and other stuff gave me nothing.
And the challenge also had a zip file that contain the code of the web page and also had a dockerfile which looked like

![Screenshot from 2024-04-17 00-35-42](https://github.com/Wizzy2323/WannaHackme/assets/159465554/ac1cb663-2997-4071-a9b1-223e2c4dc6ba)

The line 'Copy flag.txt /'   gave me some clue so I decided for path traversal for both the themes on the webpage I used the new link 
```
http://ctf.copsiitbhu.co.in:21338/?theme=/flag.txt

```
And then inspecting the new webpage give me the flag
## Flag:  COPS{path_traversal_yay_1092}


