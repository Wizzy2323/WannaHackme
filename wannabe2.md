# WannaHack CTF
> The question had the following description
```
He used to experimaent on graphs and stuff and try to draw shapes..what was the last shape drawn by him ..?

format : COPS{shape}

```
So after finding out the name of the aurthor 'BitForBat' and his github username I went to his github profile using the link 
```
github.com/BitForBat

```
After that I went to his pr1v4t3 repository and found out that the file umm.md had some mathematical equaions of the form -
$\left(\sqrt{1-x^{2}}+\ \sqrt{\left|x\right|}\right)\cdot0.8$  and 
$\left(-\sqrt{1-x^{2}}+\ \sqrt{\left|x\right|}\right)\cdot0.8$

Then I used desmos to find out that the it gave the shape of a heart
using this I solved the flag
# flag: COPS{heart}
