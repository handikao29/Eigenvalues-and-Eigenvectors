## Eigenvalues and Eigenvectors

Eigenvalues are a special set of scalars associated with a linear system of equations (i.e., a matrix equation) that are sometimes also known as characteristic roots, while eigenvectors are a special set of vectors associated with a linear system of equations that are sometimes also known as characteristic vectors

Eigenvalues and eigenvectors have a wide range of applications, for example in stability analysis, vibration analysis, atomic orbitals, facial recognition, and matrix diagonalization. 

Let there’s an _n_ × _m_ matrix can be considered as a function that uses matrix multiplication to take m-dimensional column vectors into _n_-dimensional column vectors. An _n_ × _m_ matrix is actually a linear function from _ℝ<sup>m</sup>_ to _ℝ<sup>n</sup>_. A square matrix A takes the set of n-dimensional vectors into itself, which gives a linear function from ℝn to ℝn. In this case, certain nonzero vectors **x** might be parallel to Ax, which means that a constant **λ** exists with _A_**x** = λ**x**. For these vectors, we have :

<p align="center"><i>A</i><b>x</b> = <i>λ</i><b>x</b></p>
<p align="center"><i>A</i><b>x</b> - <i>λ</i><b>x</b> = 0</p>
<p align="center"><i>A</i><b>x</b> - <i>λI</i><b>x</b> = 0</p>
<p align="center">(<i>A</i> – <i>λI</i>)<b>x</b> = 0</p>

There is a close connection between these numbers λ and the likelihood that an iterative method will converge.

If _A_ is a square matrix, the **characteristic polynomial** of _A_ is defined by
<p align="center">p(<i>λ</i>) = det(<i>A</i> - <i>λI</i>)</p>

If <i>p</i> is the characteristic polynomial of the matrix <i>A</i>, the zeros of <i>p</i> are **eigenvalues**,
or characteristic values, of the matrix <i>A</i>. If λ is an eigenvalue of _A_ and _x_ = 0 satisfies
(_A_ - _λI_)**x** = 0, then **x** is an **eigenvector**, or characteristic vector, of _A_ corresponding to the eigenvalue λ. If λ is an eigenvalue of _A_, and **x** is an eigenvector belonging to _λ_, any nonzero multiple of **x** will be an eigenvector.

<i>A</i>(<i>α</i><b>x</b>) = <i>α</i>(<i>A</i><b>x</b>) = <i>α</i>(<i>λ</i><b>x</b>) = <i>λ</i>(<i>α</i><b>x</b>)

An important consequence of this is that for any vector norm || • || we could choose the
constant _α_ = ±||**x**||-1, which would result in _α_**x** being an eigenvector with norm 1. So, for every eigenvalue and any vector norm there are eigenvectors with norm 1

To determine the eigenvalues of a matrix, we can use the fact that

• _λ_ is an eigenvalue of _A_ if and only if det(_A_ - _λI_) = 0.

Once an eigenvalue _λ_ has been found a corresponding eigenvector **x** = 0 is determined by solving the system

• (_A_ - _λI_)**x** = 0.

If **x** is an eigenvector associated with the real eigenvalue _λ_, then _A_**x** = _λ_**x**, so the matrix _A_ takes the vector **x** into a scalar multiple of itself.
• If _λ_ is real and _λ_ > 1, then _A_ has the effect of stretching **x** by a factor of _λ_.
• If 0 < _λ_ < 1, then _A_ shrinks **x** by a factor of _λ_.
• If _λ_ < 0, the effects are similar, although the direction of _A_**x** is reversed.

![Vector](https://handikao29.github.io/image/vector1.png#center)

For example, we will search all eigenvalues and eigenvectors of A = ![Matrix A](https://handikao29.github.io/image/mat1.png)

Characteristic equation to search those eigenvalues :

![Characteristic Equation](https://handikao29.github.io/image/mat2.png)

Thus, we found this eigenvalue of _A_ is _λ_=1 and _λ_=2.

An eigenvector **x**<sub>1</sub> corresponding to the eigenvalue _λ_<sub>1</sub> = 1 is a solution to the vectormatrix equation (_A_ - 1 • _I_)**x**<sub>1</sub> = 0, so

![Eigenvector x1](https://handikao29.github.io/image/mat3.png)

We found that **x**<sub>1</sub> = -**x**<sub>2</sub>. Any nonzero value of **x**<sub>1</sub> produces an eigenvector for the eigenvalue _λ_<sub>1</sub> = 1.
For example, when **x**<sub>1</sub> = 1 we have the eigenvector **x**<sub>1</sub> = (1, -1), and any eigenvector of _A_ corresponding to _λ_ = 1 is a nonzero multiple of **x**_1_.

An eigenvector **x**<sub>2</sub> corresponding to the eigenvalue _λ_<sub>2</sub> = 2 is a solution to the vectormatrix equation (_A_ - 2 • _I_)**x**<sub>2</sub> = 0, so

![Eigenvector x2](https://handikao29.github.io/image/mat4.png)

We found that **x**<sub>1</sub> = 2**x**<sub>2</sub>. Any nonzero value of **x**<sub>1</sub> produces an eigenvector for the eigenvalue _λ_<sub>2</sub> = 2.
For example, when **x**<sub>1</sub> = 1 we have the eigenvector **x**<sub>2</sub> = (2, 1), and any eigenvector of _A_ corresponding to _λ_ = 2 is a nonzero multiple of **x**<sub>2</sub>.
So, in this example, the eigenvectors which satisfy the equation is **x**<sub>1</sub> = (1,-1) with _λ_<sub>1</sub> = 1 and **x**<sub>2</sub> = (2,1) with _λ_<sub>2</sub> = 2

## Diagonalization

Diagonalization is one of eigenvalue and eigenvector’s application. It is the process of finding a corresponding diagonal matrix for a diagonalizable matrix or linear map. 
Diagonal matrix are particularly convenient for eigenvalue since the eigenvalus of diagonal matrix coincide with the diagonal entries _λ_<sub>_i_</sub> and the eigenvector corresponding the eigenvalue _λ_<sub>_i_</sub> is just the _i_<sup>th</sup> vector

![Diagonal Matrix](https://handikao29.github.io/image/diagonalmatrix.png)

This property (that the eigenvalues of diagonal matrix coincide with its diagonal entries and the eigenvectors corresponds to the corresponding coordinate vectors) is so useful and important hat in one practice often tries to make a change of coordinates just so that this will happen. But unfortunately, this isn’t always possible, if it’s possible to make a change of coordinates so that a matrix becomes diagonal we say that a matrix is diagonalizable.

Let _A_ be a real (or complex) _n_ × _n_ matrix, let _λ_<sub>1</sub>,_λ_<sub>2</sub>,_λ_<sub>3</sub>,…,_λ_<sub>n</sub> be a set of _n_ real (or complex) scalars, and let **x**<sub>1</sub>, **x**<sub>2</sub>,…,**x**<sub>n</sub> be a set of _n_ vectors ℝ<sup>n</sup> (or Cn). Let _P_ be the _n_ × _n_ matrix formed by using _x<sup>j</sup>_ for _j_<sup>th</sup> column vector and _D_ be the _n_ × _n_ diagonal matrix whose diagonal entries are the set of _n_ real (or complex) scalars. Then,

{:.center}
**AP = PD**

If and only if _λ_<sub>1</sub>,_λ_<sub>2</sub>,_λ_<sub>3</sub>,…,_λ_<sub>n</sub> are the eigenvalues of _A_ and each **x**<sub>j</sub> is and eigenvector of A corresponding the eigenvalue _λ_<sub>j</sub>.

![Proof](https://handikao29.github.io/image/proof1.png)

And so **AP = PD** implies :

![Proof2](https://handikao29.github.io/image/proof2.png)

And vice-versa.

Suppose **AP = PD**, and the matrix _P_ is invertible, thus **D = P<sup>-1</sup>AP**

A square matrix _A_ is said as diagonalizable if there exists an invertible matrix _P_ such that _P_<sup>−1</sup>_AP_ = _D_ or _PDP_<sup>-1</sup> = _A_ where _D_ is a diagonal matrix and _P_ diagonalize _A_.
If _V_ is a finite-dimensional vector space, then a linear map _T_ : _V_ → _V_ is called diagonalizable if there exists an ordered basis of _V_ with respect to which _T_ is represented by a diagonal matrix. 
The step to find invertible matrix _P_ and diagonal matrix _D_ :
```
1.	Find the eigenvalues of A.
2.	Find n linearly independent eigenvectors of A.
3.	Create P from eigenvectors in step 2.
4.	Create D with matching the eigenvalues.
```

For example, we want to find the matrix that diagonalize A = 
![Example](https://handikao29.github.io/image/mat5.png)

The diagonal matrix will be _D_ = ![Example](https://handikao29.github.io/image/mat6.png),but first, we need to find eigenvalues of _A_.

![Finding eigenvalues](https://handikao29.github.io/image/mat7.png)

So, the diagonal matrix _D_ = ![Example](https://handikao29.github.io/image/mat8.png)

In next step, we will 
