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

<div style="text-align:center"><img src ="https://github.com/handikao29/handikao29.github.io/blob/master/image/vector1.png" /></div>


## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/handikao29/handikao29.github.io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/handikao29/handikao29.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
