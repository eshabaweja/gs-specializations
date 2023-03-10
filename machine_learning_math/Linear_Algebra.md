# Linear Algebra

## Week 1

- https://www.3blue1brown.com
- Another type of problem we might be interested in is fitting an equation to some data.
- Solving **simultaneous equations**. 

- In fact, with neural networks and machine learning, we want the computer in effect not only to fit the equation, but to figure out what is the best equation to use. 
- how to find the **optimal value** of the parameters in the equation describing this line. 

### Vectors

Gaussian (Normal) Distribution

- width of sigma
- center of mu
- normalized so that it's area is 1

![image-20221221193416489](/home/eshabaweja/.config/Typora/typora-user-images/image-20221221193416489.png)

![image-20221221193935868](/home/eshabaweja/.config/Typora/typora-user-images/image-20221221193935868.png)

- in Computer Science, vectors may be represented as lists.
- Vectors can be thought of in a variety of different ways - some geometrically, some algebraically, some numerically.

![image-20221221194355394](Linear_Algebra-assets/image-20221221194355394.png)

- One of the tasks of machine learning is to **fit a model to data** in order to represent the underlying distribution.
- **keywords:** model, measured data, parameters.
- One way of fitting is to calculate the "**residuals**", which is the difference between the measured data and the modelled prediction for each histogram bin.
- A better fit would have as much **overlap** as it can, reducing the residuals as much as possible.

![img](Linear_Algebra-assets/e1_IiN-BEeiAgQrXx6bp4g_adc4beb6903f14fb5854e54714404f00_f7.png)

- The performance of a model can be quantified in a single number. One measure we can use is the *Sum of Squared Residuals*, SSR.

![img](Linear_Algebra-assets/wiqVExmsEeiahA5ak_Esmg_d0ece5b61a7d84ad7c123881e807db87_contour.png)

![image-20221221202751896](Linear_Algebra-assets/image-20221221202751896.png)

- The first goal when solving simple simultaneous equations should be to **isolate one of the variables**.
- There is also the substitution method, where we rearrange one of the equations to the form `x=ay+b` or `y=cx+d` and then substitute x or y into the other equation.
- **Vector Addition:** The head-to-tail method of adding vectors involves drawing the first vector on a graph and then placing the tail of each subsequent vector at the head of the previous vector. The **resultant** vector is then drawn from the **tail of the first** vector to the **head of the final** vector.

![image-20221221210223464](Linear_Algebra-assets/image-20221221210223464.png)

![image-20221221211547423](Linear_Algebra-assets/image-20221221211547423.png)

![image-20221221211631729](Linear_Algebra-assets/image-20221221211631729.png)

![image-20221221211842195](Linear_Algebra-assets/image-20221221211842195.png)

- vector: a list of attributes

## Week 2

### Vector Modulus

- **Orthogonal Unit Vector**:  A number of vectors that are mutually perpendicular to each other,  meaning they form an angle of 90?? with a magnitude of one unit with each other, are called orthogonal unit vectors. The dot product of an orthogonal vector is always zero since Cos90 is zero.
- Pythagoras theorem to find length of hypotenuse.

![image-20221221225922491](Linear_Algebra-assets/image-20221221225922491.png)



### Dot Product (inner scalar product; projection product)

![image-20221221230032722](Linear_Algebra-assets/image-20221221230032722.png)

- **a**???**b**=|**a**||**b**|cos(??)
- the projection of **a** along **b** is given by |**a**|cos(??), where ?? is the angle between a and b.
- we can say it is **a**???**b^** where `b^ = b/|b|` i.e. b-cap is the unit vector in b's direction
- The dot product, or inner product, of two vectors, is **the sum of the products of corresponding components**.
- https://en.wikipedia.org/wiki/Vector_projection

![image-20221222095553650](Linear_Algebra-assets/image-20221222095553650.png)

- In Trigonometry, **the law of Cosines,** also known as Cosine Rule or Cosine Formula basically relates the length of the triangle to the cosines of one of its angles. It states that, if the  length of two sides and the angle between them is known for a triangle,  then we can determine the length of the third side. It is given by:<br>

  c<sup>2</sup> = a<sup>2</sup> + b<sup>2</sup> ??? 2ab cos??<br>

  Where a, b and c are the sides of a triangle and ?? is the angle between a and b. See the figure above.

- https://www.youtube.com/watch?v=IyBINDT1ZwQ

![image-20221222101556329](Linear_Algebra-assets/image-20221222101556329.png)

![image-20221222101943042](Linear_Algebra-assets/image-20221222101943042.png)

- https://www.youtube.com/watch?v=Rw70zkvqEiE

### Changing Basis

- Change of basis is **a technique applied to finite-dimensional vector spaces in order to  rewrite vectors in terms of a different set of basis elements**. It is useful for many types of matrix computations in linear algebra and can be viewed as a type of linear transformation.
- https://www.youtube.com/watch?v=P2LTAUO1TdA
- In mathematics, **a set B of vectors in a vector space V is called a basis if every element of V may be written in a unique way as a finite linear combination of  elements of B**. The coefficients of this linear combination are referred to as components or coordinates of the vector with respect to B.
- basis is a co-ordinate system.
- **Two vectors** are linearly dependent **if and only if they are collinear**, i.e., one is a scalar multiple of the other. Any set containing the  zero vector is linearly dependent. If a subset of { v 1 , v 2 ,..., v k } is linearly dependent, then { v 1 , v 2 ,..., v k } is linearly  dependent as well.

## Week 3

### Transformations of Matrix

- https://www.gatevidyalay.com/2d-rotation-in-computer-graphics-definition-examples/

![2D Rotation in Computer Graphics | Definition | Examples | Gate Vidyalay](Linear_Algebra-assets/Rotation-Matrix-in-Computer-Graphics-1.png)

### Composition / Combination of Matrix Transformations

- The composition of matrix transformations corresponds to a notion of **multiplying two matrices together**.
- Intuitively, composition means do something, **and** then do another thing to that something.
- Formally, composition of functions is when you have two functions f and g, then  consider `g(f(x))`. We call the function `g of f` `"g composed with f"`.
  So in this video, you apply a linear transformation, which warps the space in some way, and then apply another linear transformation to the  already warped space. The result is a composition.
- https://www.khanacademy.org/math/linear-algebra/matrix-transformations/composition-of-transformations/v/compositions-of-linear-transformations-1
- https://www.123calculus.com/en/matrix-transformation-page-1-35-200.html

### Gaussian elimination and finding inverse of matrices

- In mathematics, Gaussian elimination, also known as **row reduction**, is **an algorithm for solving systems of linear equations**. It consists of a sequence of operations performed on the corresponding matrix of coefficients.
- https://www.youtube.com/watch?v=eDb6iugi6Uk

![image-20221226132450682](Linear_Algebra-assets/image-20221226132450682.png)

- elimination and back substitution
- https://www.youtube.com/watch?v=vKBNzM3V-Rc
- `inv(A)*A = I` where I is the identity matrix.

### Determinants and Inverses

- https://www.youtube.com/watch?v=3ROzG6n4yMc
- https://youtu.be/uQhTuRlWMxw
- https://en.wikipedia.org/wiki/QR_decomposition
- :link: [Help with Assignments](https://github.com/launchcode01dl/mathematics-for-machine-learning-coursera)
- https://numpy.org/

## Week 4

### Einstein summation convention

- Einstein's summation notation allows us to write this summation without the sigma notation.

![image-20221229161931197](Linear_Algebra-assets/image-20221229161931197.png)

![Einstein Summation Convention](Linear_Algebra-assets/eintein_summation_6.png)

### Using non-square matrices to do a projection

- https://www.youtube.com/watch?v=v8VSDg_WQlA

### Matrices changing basis

- https://www.youtube.com/watch?v=HZa1RwFHgwU

- Doing a transformation in a changed basis...?

### Orthogonal Matrices (orthonormal matrix)

-  A square matrix with real numbers or elements is said to be an *orthogonal matrix* if its transpose is equal to its inverse matrix.
- In linear algebra, the identity matrix of size n is the `n x n`  square matrix with ones on the main diagonal and zeros elsewhere.
- To check if a given matrix is orthogonal, first find the transpose of that matrix. Then, multiply the given matrix with the transpose. Now, if the product is an identity matrix, the given matrix is orthogonal, otherwise, not.

### The Gram???Schmidt orthonormalization process

- MIT OCW: https://www.youtube.com/watch?v=TRktLuAktBQ
