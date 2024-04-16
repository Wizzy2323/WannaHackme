# WannaHack CTF
> The following information was provided
```
Can you get admin access?

http://ctf.copsiitbhu.co.in:21340/

```
The link lead us to a web page that grants acess only to admins.
So the first thing that comes in mind while doing the web ctf is to inspect the webpage so the storage/cookies section looked like this

![Image of the cookie with the name user and the httponly value false](https://github.com/Wizzy2323/WannaHackme/assets/159465554/698129e2-fa5d-4f57-bb63-0e9c9a94a1f7)

So then I tried to change the cookie name to Admin and it worked for me to acess this web potral and get the flag

## Flag:  COPS{broken_auth_using_cookies_231} .


