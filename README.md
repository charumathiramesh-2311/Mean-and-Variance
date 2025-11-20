#  Mean and variance of a discrete  distribution


# Aim : 

To find mean and variance of arrival of objects from the feeder using probability distribution


# Software required :  

Python and Visual components tool

# Theory:

The expectation or the mean of a discrete random variable is a weighted average of all possible
values of the random variable. The weights are the probabilities associated with the corresponding values. 
It is calculated as,

![image](https://user-images.githubusercontent.com/103921593/192938463-e34177f4-f188-48a0-bda2-8f6d1d660ed2.png)

The variance of a random variable shows the variability or the scatterings of the random variables.
It shows the distance of a random variable from its mean. It is calcualted as

![image](https://user-images.githubusercontent.com/103921593/192938695-99fedc01-34d5-4d36-84df-5880e766ed0c.png)


# Algorithm:

1.

<br>

2.

<br>

3.

<br>

4.

<br>

5.

<br>

# Experiment :

![image](https://user-images.githubusercontent.com/103921593/229993174-5b67e57e-3e01-4ac4-9f83-410a932b22bf.png)

# Program :
```c
#Developed by : CHARUMATHI R
#Register No : 212222240021
import numpy as np
L=[int(i) for i in input().split()]
N=len(L); M=max(L)
x=list();f=list()
for i in range (M+1):
    c = 0
    for j in range(N):
        if L[j]==i:
            c=c+1
    f.append(c)
    x.append(i)
sf=np.sum(f)
p=list()
for i in range(M+1):
    p.append(f[i]/sf)
mean=np.inner(x,p)
EX2=np.inner(np.square(x),p)
var=EX2-mean**2
SD=np.sqrt(var)
print("The Mean arrival rate is %.3f " %mean)
print("The Variance of arrival from feeder is %.3f " %var)
print("The Standard deviation of arrival from feeder is %.3F " %SD)
```


# Output : 

<p></p>
<br>
<p></p>
<br>










# Results :






