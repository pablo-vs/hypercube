#Hypercube

A proof-of-concept for the Dimension project (https://github.com/pablo-vs/dimension)  

Displays a 3D projection of an N-dimensional hypercube and allows to rotate any pair of its coordinates. By default N=5, but this can be changed in the source code.  

Usage: clone the repository and run start.sh  
```
git clone https://github.com/pablo-vs/hypercube
cd hypercube
./start.sh
```

You will see three slides in the sides and bottom, and a selector in the top

![alt text](https://github.com/pablo-vs/hypercube/screenshot2.png)

The bottom and right slides control rotation of the 3D projection, the left slide controls rotation of the pair of coordinates selected in the top control. For this 5 dimensional example, coordinates 2, 3 and for are projected to the 3D space and thus any rotation involving only those axes will result in a boring 3d rotation. Rotations along coordinates 0 and 1 are completely beyond 3D space and will show up as a change in size of the different cubes which appear to form the hypercube. Mixed rotations (eg 12) will show up as a change in shape.

You can change the dimensionality by modifying the dim constant in main() and recompiling. You will probably need to adjust the scale too. In my computer it works fine up to 10 dimensions, but it becomes too slow with higher numbers.


![alt text](https://github.com/pablo-vs/hypercube/screenshot1.png)
