# Vectors: Geometric View

## Definition of Vectors

> **Definition 1.1.1 Vectors**
> 
> Quantities that have both a **magnitude** (the "how much" or "how big" part) and a **direction** in space. The magnitude of a vector is also called its **norm** or **length**.

Regarding the notation of vectors, different books or authors have different habits. You may see **A** (boldface letter), $\overrightarrow{A}$ (with an arrow above), $\overrightarrow{\textbf{A}}$ (both boldface and arrow) etc. I will stick to $\overrightarrow{A}$, because I like using boldface letters to make readers pay attention to those words. Formally, we have:

- Position vector of point $A$ which starts at the origin: $\overrightarrow{OA}$. We denote its magnitude as $|\overrightarrow{OA}|$[^1] or $OA$.
- Displacement vector of $B$ relative to $A$: $\overrightarrow{AB}$. Its length is $|\overrightarrow{AB}|$.

Finally, we say **two vectors are equal** if they have the same magnitude and direction, and **the negative of a vector $\overrightarrow{a}$** is the vector parallel to $\overrightarrow{a}$ with the same length but in the opposite direction. It is denoted $-\overrightarrow{a}$.

## Basic Operations

In this part, I want to briefly talk about vector addition (subtraction) and vector multiplication by a scalar. As this is just a note, I will only give you some schematic diagrams[^2]:


<div style="display: flex; justify-content: space-around;">
    <div style="flex: 1; text-align: center;">
        <img src="1.png" alt="Vector Addition" style="width: 100%;">
        <p style="text-align: center;"><em>Figure 1</em></p>
    </div>
    <div style="flex: 1; text-align: center;">
        <img src="2.png" alt="Vector Subtraction" style="width: 100%;">
        <p style="text-align: center;"><em>Figure 2</em></p>
    </div>
</div>
<div style="text-align: center; margin-top: 20px;">
    <img src="3.png" alt="Vector Scalar Multiplication" style="width: 70%;">
    <p style="text-align: center;"><em>Figure 3</em></p>
</div>

Pictures above show the way we perform vector addition or subtraction. An interesting fact is that $\overrightarrow{BA}$, which is the sum of two vectors, is a diagonal of a parallelogram. However, as Figure 3 shows, the subtraction is another diagonal.

For a vector multiplied by a scalar, it's just a stretching or compressing of the vector, omitted here. But one thing is important:

> Theorem 1.2.1: Parallel
>
>Two non-zero vectors are parallel if and only if one is a scalar multiple of the other, i.e.
> 
> $$\begin{equation}\overrightarrow{a} \parallel \overrightarrow{b} \Leftrightarrow \overrightarrow{a} = \lambda \overrightarrow{b}. \tag{1.1} \end{equation}$$


## The Scalar Product

> **Definition 1.3.1: The Scalar Product**
> 
> The scalar product, also called dot product or inner product of two vectors, say $\overrightarrow{a}, \overrightarrow{b}$ is defined as:
> 
> $$\begin{equation}\overrightarrow{a} \cdot \overrightarrow{b} = |\overrightarrow{a}||\overrightarrow{b}|\cos \theta\tag{1.2}\end{equation}$$
> Here, $\theta$ is the small angle between the two vectors (ranges from $0$ to $\pi$).

We have another definition: (forgive my laziness)

> **Definition 1.3.2: Components** [^3]
<div style="text-align: center;">
    <img src="14.png" alt="Components" style="width: 100%;">
    <p style="text-align: center;"><em>Figure 4</em></p>
</div>

Please notice that a component is a scalar! If you want the vector along the direction of $\overrightarrow{b}$ with a magnitude as the component of $\overrightarrow{a}$ in the direction of $\overrightarrow{b}$, what you are searching for is a concept called projection:

> **Definition 1.3.3: Projection**
> 
> $$\begin{equation}\text{Projection of } \overrightarrow{a} \text{ onto } \overrightarrow{b} = \frac{\overrightarrow{a} \cdot \overrightarrow{b}}{|\overrightarrow{b}|}\overrightarrow{b}\tag{1.3}\end{equation}$$

There is a useful schematic diagram for the scalar product[^4]:

<div style="display: flex; justify-content: space-around;">
    <div style="flex: 1; text-align: center;">
        <img src="4.png" alt="Diagram 1" style="width: 100%;">
        <p style="text-align: center;"><em>Figure 5</em></p>
    </div>
    <div style="flex: 1; text-align: center;">
        <img src="5.png" alt="Diagram 2" style="width: 100%;">
        <p style="text-align: center;"><em>Figure 6</em></p>
    </div>
    <div style="flex: 1; text-align: center;">
        <img src="6.png" alt="Diagram 3" style="width: 100%;">
        <p style="text-align: center;"><em>Figure 7</em></p>
    </div>
</div>

This shows that the sign of the scalar product reveals the angle between two vectors. If the value of the scalar product is positive, the angle will be acute; negative for an obtuse angle; 0 for a right angle. Actually, we have:

> Theorem 1.3.4: Angle between Vectors
>
> $$\begin{equation}\cos \theta = \frac{\overrightarrow{a} \cdot \overrightarrow{b}}{|\overrightarrow{a}||\overrightarrow{b}|}\tag{1.4}\end{equation}$$

Some special cases need us to pay more attention:

> Theorem 1.3.5: Perpendicular and Parallel
>
> $$\begin{align}\overrightarrow{a} \perp \overrightarrow{b} \Leftrightarrow \overrightarrow{a} \cdot \overrightarrow{b} = 0\tag{1.5}\\
> \overrightarrow{a} \parallel \overrightarrow{b} \Leftrightarrow|\overrightarrow{a} \cdot \overrightarrow{b}| = |\overrightarrow{a}||\overrightarrow{b}|\tag{1.6}\end{align}$$

We will see more applications of the scalar product when introducing the Cartesian coordinate system. Just wait and see.

## The Vector Product

> **Definition 1.4.1: The Vector Product**
> 
> We denote the vector product of two vectors $\overrightarrow{a}, \overrightarrow{b}$, also called cross product, by $\overrightarrow{a} \times \overrightarrow{b}$. The result of it is a vector, and we define it by defining its magnitude and direction:
> - **Magnitude:**
> 
> $$
> \begin{equation}\left|\overrightarrow{a} \times \overrightarrow{b}\right| = |\overrightarrow{a}||\overrightarrow{b}|\sin \theta \tag{1.7}\end{equation}$$
> - **Direction:** $\overrightarrow{a} \times \overrightarrow{b}$ is perpendicular to the plane formed by $\overrightarrow{a}$ and $\overrightarrow{b}$, using the **right-hand rule** to choose the final direction.

At first glance, the definition of vector product is kind of complex, but there are also helpful schematic diagrams[^5]:

<div style="text-align: center;">
    <img src="7.png" alt="Magnitude of Vector Product" style="width: 60%;">
    <p style="text-align: center;"><em>Figure 8</em></p>
</div>

<div style="display: flex; justify-content: space-around;">
    <div style="flex: 1; text-align: center;">
        <img src="8.png" alt="Right-Hand Rule 1" style="width: 60%;">
        <p style="text-align: center;"><em>Figure 9</em></p>
    </div>
    <div style="flex: 1; text-align: center;">
        <img src="9.png" alt="Right-Hand Rule 2" style="width: 60%;">
        <p style="text-align: center;"><em>Figure 10</em></p>
    </div>
</div>

Figure 8 shows that the magnitude of the vector product is the area of the parallelogram "spanned" by the two vectors. Then Figures 9 and 10 show you how the right-hand rule works. Notice that I have been ignoring the rules of operations of vectors, like the commutative law of vector addition, etc. The reason is that most of them are like the rules for numbers. However, the only difference just showed up, we have:

> Theorem 1.4.2: Anticommutative Law of Vector Product
>
> $$
> \begin{equation}
>    \overrightarrow{a} \times \overrightarrow{b} = -\overrightarrow{b} \times \overrightarrow{a}\tag{1.8}
> \end{equation}$$

Vectors can be more applicable, but we have to bring something up here. Don't worry, it is Mr. Descartes who comes to help.


# Vectors with Cartesian Coordinate

## Introducing Cartesian Coordinates

I believe the readers are quite familiar with the Cartesian coordinate system, so I just want to show you two graphs of it[^6]:

<div style="display: flex; justify-content: space-around;">
    <div style="flex: 1; text-align: center;">
        <img src="10.png" alt="Cartesian Coordinate 1" style="width: 70%;">
        <p style="text-align: center;"><em>Figure 11</em></p>
    </div>
    <div style="flex: 1; text-align: center;">
        <img src="11.png" alt="Cartesian Coordinate 2" style="width: 70%;">
        <p style="text-align: center;"><em>Figure 12</em></p>
    </div>
</div>

Here, only a little knowledge needs to be introduced:

> **Definition 2.1.1: Unit Vector and $\overrightarrow{i}, \overrightarrow{j}, \overrightarrow{k}$**
> 
> **A unit vector is a vector that has a magnitude of 1**, its only purpose is to point—that is, to describe a direction in space.
> 
> In an xy-coordinate system, we can define a unit vector $\overrightarrow{i}$ **that points in the direction of the positive x-axis** and a unit vector $\overrightarrow{j}$ **that points in the direction of the positive y-axis**. If we are dealing with a xyz-coordinate, we define a unit vector $\overrightarrow{k}$ **that points in the direction of the positive z-axis**.
> 
> <div style="display: flex; justify-content: space-around;">
>     <div style="flex: 1; text-align: center;">
>         <img src="16.png" alt="XY Coordinate" style="width: 70%;">
>         <p style="text-align: center;"><em>Figure 13</em></p>
>     </div>
>     <div style="flex: 1; text-align: center;">
>         <img src="17.png" alt="XYZ Coordinate" style="width: 70%;">
>         <p style="text-align: center;"><em>Figure 14</em></p>
>     </div>
> </div>

## Converting

Now, a critical problem: if we know a vector, which means we know its magnitude and direction, how can we represent it in the Cartesian coordinate system? Here suppose the meaning of the direction of a vector is denoted by the angle between the vector and x-axis, which is $\theta$. This means we have[^7]:

<div style="text-align: center;">
    <img src="12.png" alt="Vector Conversion" style="width: 40%;">
    <p style="text-align: center;"><em>Figure 15</em></p>
</div>

In the picture above, we have a vector $\overrightarrow{A}$ with magnitude $|\overrightarrow{A}|$, so it is easy to find its component on the x-axis is $|\overrightarrow{A}|\cos \theta$ and the component on the y-axis is $|\overrightarrow{A}|\sin \theta$. Thus, by vector addition we have:

$$
\begin{equation}
    \overrightarrow{A} = |\overrightarrow{A}|\cos \theta \overrightarrow{i} + |\overrightarrow{A}|\sin \theta \overrightarrow{j} \tag{2.1}
\end{equation}
$$

Then, we write:

$$
\begin{equation}
    \overrightarrow{A} = 
    \begin{pmatrix}
        |\overrightarrow{A}|\cos \theta \\
        |\overrightarrow{A}|\sin \theta
    \end{pmatrix}\tag{2.2}
\end{equation}
$$

Some books prefer:

$$
\begin{bmatrix}
        \left|\overrightarrow{A}\right|\cos \theta	\\
        \left|\overrightarrow{A}\right|\sin \theta
    \end{bmatrix}
 $$

Here, let $A_x = |\overrightarrow{A}|\cos \theta, A_y = |\overrightarrow{A}|\sin \theta$. By applying the Pythagorean theorem, we have:

> **Theorem 2.2.1: The Magnitude of Vectors**
> 
> $$\begin{equation} |\overrightarrow{A}| = \sqrt{A_x^2 + A_y^2}\tag{2.3}\end{equation}$$
> 
> It is not hard to see that in xyz-coordinates, the formula would be:
> 
> $$\begin{equation}|\overrightarrow{A}| = \sqrt{A_x^2 + A_y^2 + A_z^2}\tag{2.4}\end{equation}$$

A numerical example[^8]:

<div style="text-align: center;">
    <img src="13.png" alt="Numerical Example" style="width: 25%;">
    <p style="text-align: center;"><em>Figure 16</em></p>
</div>

$$
\text{Here } \overrightarrow{OP} = 2\overrightarrow{i} + 5\overrightarrow{j}, \text{ hence } \overrightarrow{OP} =
\begin{pmatrix}
    2 \\
    5
\end{pmatrix}
\text{ and } |\overrightarrow{OP}| = \sqrt{2^2 + 5^2} = \sqrt{29}.
$$

What I mean by this subsection is that when we write a vector as something like

$$
\overrightarrow{A} = 
\begin{pmatrix}
  2 \\
  5
\end{pmatrix},
$$

what we really mean is that $\overrightarrow{A} = 2\overrightarrow{i} + 5\overrightarrow{j}$.


## "Translating"

We finally made it here. The final task is to "translate" things from the previous sections into coordinates.

Suppose we have three vectors:

$$
\overrightarrow{a} = 
\begin{pmatrix}
    a_1 \\
    a_2 \\
    a_3
\end{pmatrix},\quad
\overrightarrow{b} = 
\begin{pmatrix}
    b_1 \\
    b_2 \\
    b_3
\end{pmatrix},\quad
\overrightarrow{c} = 
\begin{pmatrix}
    c_1 \\
    c_2 \\
    c_3
\end{pmatrix}
$$

- $\overrightarrow{a} = \overrightarrow{b} \Leftrightarrow a_1 = b_1, a_2 = b_2, a_3 = b_3$
- Negative:

$$-\overrightarrow{a} = -\begin{pmatrix}
    a_1 \\
    a_2 \\
    a_3
\end{pmatrix} = \begin{pmatrix}
    -a_1 \\
    -a_2 \\
    -a_3
\end{pmatrix}$$

- Addition:

$$\overrightarrow{a} + \overrightarrow{b} = \begin{pmatrix}
    a_1 + b_1 \\
    a_2 + b_2 \\
    a_3 + b_3
\end{pmatrix}$$

Let me prove the third one to you:

$$
\overrightarrow{a} + \overrightarrow{b} = a_1 \overrightarrow{i} + a_2 \overrightarrow{j} + a_3 \overrightarrow{k} + b_1 \overrightarrow{i} + b_2 \overrightarrow{j} + b_3 \overrightarrow{k} \\
= (a_1 + b_1) \overrightarrow{i} + (a_2 + b_2) \overrightarrow{j} + (a_3 + b_3) \overrightarrow{k} \\
= \begin{pmatrix}
    a_1 + b_1 \\
    a_2 + b_2 \\
    a_3 + b_3
\end{pmatrix}
$$

The proof of other results usually follows the same idea, so I will just list the results here now:

- $\overrightarrow{a} \parallel \overrightarrow{b} \Leftrightarrow a_1 = \lambda b_1, a_2 = \lambda b_2, a_3 = \lambda b_3$
- $\overrightarrow{a} \cdot \overrightarrow{b} = a_1 b_1 + a_2 b_2 + a_3 b_3$
- $|\overrightarrow{a}| = \sqrt{\overrightarrow{a} \cdot \overrightarrow{a}} = \sqrt{a_1^2 + a_2^2 + a_3^2}$
- By the way, if we want to find a unit vector whose direction is the same as $\overrightarrow{a}$, we can have $\displaystyle \frac{1}{|\overrightarrow{a}|}\overrightarrow{a}$
- $\cos \theta = \displaystyle \frac{a_1 b_1 + a_2 b_2 + a_3 b_3}{\sqrt{a_1^2 + a_2^2 + a_3^2} \sqrt{b_1^2 + b_2^2 + b_3^2}}$
- $\overrightarrow{a} \perp \overrightarrow{b} \Leftrightarrow a_1 b_1 + a_2 b_2 + a_3 b_3 = 0$

The vector product or the cross product is a little bit more complex:

$$
\begin{array}{c}
\overrightarrow{a} \times \overrightarrow{b} = (a_1 \overrightarrow{i} + a_2 \overrightarrow{j} + a_3 \overrightarrow{k}) \times (b_1 \overrightarrow{i} + b_2 \overrightarrow{j} + b_3 \overrightarrow{k}) \\
= a_1 b_1 \overrightarrow{i} \times \overrightarrow{i} + a_1 b_2 \overrightarrow{i} \times \overrightarrow{j} + a_1 b_3 \overrightarrow{i} \times \overrightarrow{k} \\
\qquad + a_2 b_1 \overrightarrow{j} \times \overrightarrow{i} + a_2 b_2 \overrightarrow{j} \times \overrightarrow{j} + a_2 b_3 \overrightarrow{j} \times \overrightarrow{k} \\
\qquad \quad + a_3 b_1 \overrightarrow{k} \times \overrightarrow{i} + a_3 b_2 \overrightarrow{k} \times \overrightarrow{j} + a_3 b_3 \overrightarrow{k} \times \overrightarrow{k}
\end{array}
$$

Please note that, by applying the definition 1.4.1 and the Anticommutative law 1.4.2, we have:

$$
\begin{array}{c}
    \overrightarrow{i} \times \overrightarrow{i} = \overrightarrow{0}, \overrightarrow{j} \times \overrightarrow{j} = 0, \overrightarrow{k} \times \overrightarrow{k} = 0 \\
    \overrightarrow{i} \times \overrightarrow{j} = \overrightarrow{k}, \overrightarrow{j} \times \overrightarrow{i} = -\overrightarrow{k} \\
    \overrightarrow{i} \times \overrightarrow{k} = -\overrightarrow{j}, \overrightarrow{k} \times \overrightarrow{i} = \overrightarrow{j} \\
    \overrightarrow{j} \times \overrightarrow{k} = \overrightarrow{i}, \overrightarrow{k} \times \overrightarrow{j} = -\overrightarrow{i}
\end{array}
$$

So continuing our calculation, we will have:

$$
\begin{array}{c}
\overrightarrow{a} \times \overrightarrow{b} = a_1 b_2 \overrightarrow{k} - a_1 b_3 \overrightarrow{j} - a_2 b_1 \overrightarrow{k} + a_2 b_3 \overrightarrow{i} + a_3 b_1 \overrightarrow{j} - a_3 b_2 \overrightarrow{i} \\
= (a_2 b_3 - a_3 b_2) \overrightarrow{i} + (a_3 b_1 - a_1 b_3) \overrightarrow{j} + (a_1 b_2 - a_2 b_1) \overrightarrow{k} \\
= \begin{pmatrix}
    a_2 b_3 - a_3 b_2 \\
    a_3 b_1 - a_1 b_3 \\
    a_1 b_2 - a_2 b_1
\end{pmatrix}
\end{array}
$$

It is hard to remember this result, but if you know determinants, then we can actually write it in another way:

$$
\begin{equation}
    \overrightarrow{a} \times \overrightarrow{b} =
    \begin{vmatrix}
        \overrightarrow{i} & \overrightarrow{j} & \overrightarrow{k} \\
        a_1 & a_2 & a_3 \\
        b_1 & b_2 & b_3
    \end{vmatrix}\tag{2.5}
\end{equation}
$$


## Triple Product

We have the so-called triple product, which is $\overrightarrow{c} \cdot (\overrightarrow{a} \times \overrightarrow{b})$ or $(\overrightarrow{a} \times \overrightarrow{b}) \cdot \overrightarrow{c}$ (they are the same because the dot product has the commutative law):

> **Definition 2.4.1: Triple Product**
> 
> For the value of the triple product, we have:
> 
> $$
> \begin{equation}
>    \overrightarrow{c} \cdot (\overrightarrow{a} \times \overrightarrow{b}) = |\overrightarrow{c}||(\overrightarrow{a} \times \overrightarrow{b})|\cos \psi\tag{2.6}
> \end{equation}$$
> 
> Here, $\psi$ is the angle between $\overrightarrow{c}$ and $(\overrightarrow{a} \times \overrightarrow{b})$. Or, in coordinates, using the determinant, we have:
> 
> $$
> \begin{equation}
>    \overrightarrow{c} \cdot (\overrightarrow{a} \times \overrightarrow{b}) =
>    \begin{vmatrix}
>        c_1 & c_2 & c_3 \\
>        a_1 & a_2 & a_3 \\
>        b_1 & b_2 & b_3
>    \end{vmatrix}\tag{2.7}
> \end{equation}$$
> 
> The key thing is that there is a geometric meaning to the triple product: its absolute value is the volume of the parallelepiped[^9]:
> 
> <div style="text-align: center;">
>     <img src="15.png" alt="Parallelepiped" style="width: 20%;">
>     <p style="text-align: center;"><em>Figure 17</em></p>
> </div>
> 
> This is because $|\overrightarrow{c}|\cos \psi$ is actually the height of the parallelepiped, while $|(\overrightarrow{a} \times \overrightarrow{b})|$ is the area of the base of the parallelepiped. Hence, it is obvious to see it.


# $\ ^\ast$Epilogue

## Inequalities

Using the dot product (scalar product), we can prove two famous and important inequalities:

> **Theorem 3.1.1: Cauchy-Schwarz Inequalities**
>
> $$
\begin{equation}
    \sum_{i=1}^{3} x_i y_i \le \sqrt{\sum_{i=1}^{3} x_i^2} \sqrt{\sum_{i=1}^{3} y_i^2} \tag{3.1}
\end{equation}
$$

**Proof:**
Let

$$
\begin{equation*}
\overrightarrow{x} = 
\begin{pmatrix}
x_1 \\
x_2 \\ 
x_3
\end{pmatrix}\quad \text{and}\quad
\overrightarrow{y} =
\begin{pmatrix}
y_1\\
y_2 \\
y_3
\end{pmatrix}
\end{equation*}
$$

We have:

$$
\cos \theta = \frac{x_1 y_1 + x_2 y_2 + x_3 y_3}{\sqrt{x_1^2 + x_2^2 + x_3^2} \sqrt{y_1^2 + y_2^2 + y_3^2}}
$$

Clearly, $\cos \theta \le 1$. Hence,

$$
\frac{x_1 y_1 + x_2 y_2 + x_3 y_3}{\sqrt{x_1^2 + x_2^2 + x_3^2} \sqrt{y_1^2 + y_2^2 + y_3^2}} \le 1
$$

Which is what we want:

$$
\sum_{i=1}^{3} x_i y_i \le \sqrt{\sum_{i=1}^{3} x_i^2} \sqrt{\sum_{i=1}^{3} y_i^2}
$$

Maybe you are more familiar with this inequality when we are in a 2-D plane, but the result and proof are pretty similar. Actually, the generalized version of it should be:

$$
\begin{equation}
    \sum_{i=1}^{n} x_i y_i \le \sqrt{\sum_{i=1}^{n} x_i^2} \sqrt{\sum_{i=1}^{n} y_i^2}\tag{3.2}
\end{equation}
$$

You can prove it using a similar method here as long as you think or "believe" there is an angle in $n$-dimensional space. Otherwise, you shall use some other method. I put this here because I usually forget this important inequality, but with vectors, it is quite easy to remember, just:

$$
\begin{equation}
    \overrightarrow{x} \cdot \overrightarrow{y} \le |\overrightarrow{x}| |\overrightarrow{y}|\tag{3.3}
\end{equation}
$$

Another important inequality is:

> **Theorem 3.1.2: Triangle Inequality**
>
> $$
> \begin{equation}
>    |\overrightarrow{x} + \overrightarrow{y}| \le |\overrightarrow{x}| + |\overrightarrow{y}|\tag{3.4}
> \end{equation}$$

**Proof:**
We have:

$$
\begin{align*}
    (|\overrightarrow{x} + \overrightarrow{y}|)^2 &= (\overrightarrow{x} + \overrightarrow{y}) \cdot (\overrightarrow{x} + \overrightarrow{y}) \\
    &= |\overrightarrow{x}|^2 + 2 \overrightarrow{x} \cdot \overrightarrow{y} + |\overrightarrow{y}|^2 \\
    &\le |\overrightarrow{x}|^2 + 2 |\overrightarrow{x}| |\overrightarrow{y}| + |\overrightarrow{y}|^2 \\
    &= (|\overrightarrow{x}| + |\overrightarrow{y}|)^2
\end{align*}
$$

Hence, we have:

$$
(|\overrightarrow{x} + \overrightarrow{y}|)^2 \le (|\overrightarrow{x}| + |\overrightarrow{y}|)^2
$$

Notice that both $|\overrightarrow{x} + \overrightarrow{y}|$ and $|\overrightarrow{x}| + |\overrightarrow{y}|$ are non-negative numbers, and we have a trivial result that if $a^2 \le b^2$ then $a \le b$ provided $a \ge 0, b \ge 0$. So we have:

$$
|\overrightarrow{x} + \overrightarrow{y}| \le |\overrightarrow{x}| + |\overrightarrow{y}|
$$

Forget about the proof for a second. Notice that this inequality just says that **the length of one side of a triangle cannot be longer than the sum of the lengths of the other two sides** (See Figure 1). Which you should have learned in your younger age.

## Direction Cosine

Some books might also introduce the concepts of direction angles and direction cosine:

> **Definition 3.2.1: Direction Angles and Direction Cosine**
>
> The **direction angles** of a vector $\overrightarrow{a}$ is the angle between $\overrightarrow{a}$ and $\overrightarrow{i}, \overrightarrow{j}, \overrightarrow{k}$, i.e., the angle between the vector and the three positive coordinate axes. **Commonly, they will be denoted by $\alpha$ (between x-axis), $\beta$ (between y-axis), $\gamma$ (between z-axis)**. The **direction cosines** (or directional cosines) of a vector are the cosines of the angles between the vector and the three positive coordinate axes.

Using the dot product, the direction cosines are not hard to calculate. Let

$$
\overrightarrow{a} =
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
$$

$$
\begin{align}
    \cos \alpha = \frac{\overrightarrow{a} \cdot \overrightarrow{i}}{|\overrightarrow{a}||\overrightarrow{i}|} = \frac{x}{\sqrt{x^2 + y^2 + z^2}} \tag{3.5}\\
    \cos \beta = \frac{\overrightarrow{a} \cdot \overrightarrow{j}}{|\overrightarrow{a}||\overrightarrow{j}|} = \frac{y}{\sqrt{x^2 + y^2 + z^2}} \tag{3.6}\\
    \cos \gamma = \frac{\overrightarrow{a} \cdot \overrightarrow{k}}{|\overrightarrow{a}||\overrightarrow{k}|} = \frac{z}{\sqrt{x^2 + y^2 + z^2}}\tag{3.7}
\end{align}
$$

Two interesting things here, first:

$$
\begin{equation}
    {\cos \alpha}^2 + {\cos \beta}^2 + {\cos \gamma}^2 = 1\tag{3.8}
\end{equation}
$$

Second, we have said in a previous section that to find a unit vector whose direction is the same as $\overrightarrow{a}$, we just need $\displaystyle \frac{1}{|\overrightarrow{a}|} \overrightarrow{a}$. Here it should be:

$$
\frac{1}{|\overrightarrow{a}|} \overrightarrow{a} = \frac{1}{\sqrt{x^2 + y^2 + z^2}}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix} = 
\begin{pmatrix}
\frac{x}{\sqrt{x^2 + y^2 + z^2}} \\
\frac{y}{\sqrt{x^2 + y^2 + z^2}} \\
\frac{z}{\sqrt{x^2 + y^2 + z^2}}
\end{pmatrix}
$$

Do you see that? We just found that:

$$
\begin{equation}
    \text{The unit vector for } \overrightarrow{a}: \frac{1}{|\overrightarrow{a}|} \overrightarrow{a} =
    \begin{pmatrix}
    \cos \alpha \\
    \cos \beta \\
    \cos \gamma
    \end{pmatrix}\tag{3.9}
\end{equation}
$$

[^1]: Some books might use the symbol $\|\overrightarrow{OA}\|$ for the magnitude of a vector.

[^2]: The three pictures all come from the book *The Mechanical Universe: Mechanics and Heat* by Steven C. Frautschi, Richard P. Olenick, Tom M. Apostol, and David L. Goodstein.

[^3]: The source of the figure is *Mathematics Application and Interpretation HL 2* by Michael Haese, Mark Humphries, Chris Sangwin, and Ngoc Vo.

[^4]: These three pictures comes from *University Physics with Modern Physics* (14th ed.) by Young and Freedman

[^5]: The source of the first two figures is *The Mechanical Universe: Mechanics and Heat* by Steven C. Frautschi, Richard P. Olenick, Tom M. Apostol, and David L. Goodstein, and the source of the last two figures is *University Physics with Modern Physics* (14th ed.) by Young and Freedman.

[^6]: The source of the two figures is *The Mechanical Universe: Mechanics and Heat* by Steven C. Frautschi, Richard P. Olenick, Tom M. Apostol, and David L. Goodstein.

[^7]: The source of the figure is *University Physics with Modern Physics* (14th ed.) by Young and Freedman.

[^8]: The source of the figure is *Mathematics Application and Interpretation HL 2* by Michael Haese, Mark Humphries, Chris Sangwin, and Ngoc Vo.

[^9]: The source of the figure is 《解析几何（第三版）》by 丘维声.
