HW3-Problem5
============
This method multiplies two matrices together and returns their product.


Example:

from sage.all import matrix
A = Matrix([[1,2,3,4],[5,6,7,8],[9,10,11,12],[13,14,15,16]])
B = Matrix([[1,0,0,2],[0,3,5,4],[9,2,5,3],[3,0,1,0]])

get_product(A, B) -->
[ 40  12  29  19]
[ 92  32  73  55]
[144  52 117  91]
[196  72 161 127]


Timings:

code in python: timeit("get_product(A, B)") --> 625 loops, best of 3: 13.8 µs per loop

code in cython: timeit("get_product(A, B)") --> 625 loops, best of 3: 13.5 µs per loop
