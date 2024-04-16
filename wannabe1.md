# WannaHack CTF
> We were given the following details
```
This photo is the last evidence of my friend..help me find out more about him..

Whats his github username?

Flag format: COPS{username}
```
![This was the image file](https://github.com/Wizzy2323/WannaHackme/assets/159465554/58d48082-81fd-4693-9801-f6dc3ffa6683)

using the exiftool 
```
exiftool filename
```
I got aurthor name 'Qml0Rm9yQmF0'
I wasted a lot of time in serching about this aurthor until I came to know that it was base64 encoding decoding it gave the name 'BitForBat'
Which soved this question
# flag:COPS{BitForBat}
