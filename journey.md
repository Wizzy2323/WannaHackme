# WannaHack CTF
> we were provided with the following information
```
Are you ready to start the journey?

Follow the instructions in instructions.mp3

And we were given with a image file and and audio file

```
![This was the image file](https://github.com/Wizzy2323/WannaHackme/assets/159465554/b5331893-38aa-4822-b040-11a1511c5473)

```
And the audio file told that that the image file was divided into three parts and the image file said that 'The password is of the form journey_???? '
So I went for Audio Stegnography but found nothing from the mp3 audio
then i went to apply my forensic skills in the image file.

```
>using exiftool i got the first part of the flag in the comment section
# flag1 : COPS{f1rst_
```
now for the second part we had to binwalk the file to extract the the data
the command line for the same is binwalk -e filename

```
after this we had a new directory which had an zip file which was password protected for which we apply john the ripper using the commands-
```
john-the-ripper.zip2john filename > hash
&
john-the-ripper --wordlist=pass.txt hash

```
The pass.txt file can be made by simply using a loop program to store all the permutation of the password
The final password was 
# password = journey_1503
Now unziping the zip file 5E70.zip and entering the right password it had an image file 

using strings command 'stirngs imagefile' it had a base64 string hidden which was 'czNjMG5kXw==' identified with two equal signs at the end which gave the second part of the flag
# flag2 : s3c0nd_
Now the third part of the flag was got with applying foremost on the hidden image file the that gave an output folder which had another image file which gave the third part of the flag
![The third flag file](https://github.com/Wizzy2323/WannaHackme/assets/159465554/cf36347d-ace6-4d3c-8f18-731bb59b7fed)

# flag3 : th1rd_696}
Hence The final flag was
# flag : COPS{f1rst_s3cond_th1rd_696}
