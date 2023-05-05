# **Matrices in Linear Algebra: Objects that operate on Vectors**

- <details close><summary><h2>Practice Quiz 1 : Using matrices to make transformations</h2></summary>

    ### <span style="color: green;">**Congratulations! You passed!**</span>

    #### **Grade received** <span style="color: green;">100%</span>

    #### **Latest Submission Grade** 100%

    #### **To pass** 80% or higher

    ---

    1. Matrices make transformations on vectors, potentially changing their magnitude and direction.

        If we have two unit vectors (in orange) and another vector, 
        $\begin{bmatrix}
            3 \\
            2
        \end{bmatrix}$
        (in pink), before any transformations - these look like this:

        ![q11.png](img/q11.png)

        Take the matrix,
        $A = \begin{bmatrix}
            1/2 & -1 \\
            0 & 3/4
        \end{bmatrix}$
        , see how it transforms the unit vectors and the vector $r$,

        ![q12.png](img/q12.png)

        What new vector $r^{'}$, does $A$ transform $r$ to? Specially, what does the following equal?

        $$Ar=\begin{bmatrix}
            1/2 & -1 \\
            0 & 3/4
        \end{bmatrix}\begin{bmatrix}
            3 \\
            2
        \end{bmatrix} =$$

    - [x] 
    $\begin{bmatrix}
        -1/2 \\
        3/2
    \end{bmatrix}$
    - [ ] 
    $\begin{bmatrix}
        -3/2 \\
        3/2
    \end{bmatrix}$
    - [ ] 
    $\begin{bmatrix}
        3/2 \\
        -1/2
    \end{bmatrix}$
    - [ ] 
    $\begin{bmatrix}
        3/2 \\
        -3/4
    \end{bmatrix}$

        > ✔️ <spane style="color: green;">**Correct**</br>You could either calculate this or read it off the graph.</span>

    ---

    2. Let's use the same matrix
    $A = \begin{bmatrix}
        1/2 & -1 \\
        0 & 3/4
    \end{bmatrix}$
    from the previous question.

        Type an expression for the vector
        $s = A\begin{bmatrix}
            -2 \\
            4
        \end{bmatrix}$

        ```python
        s = [-5, 3]
        ```

        > ✔️ <spane style="color: green;">**Correct**</br>Well done</span>

    ---

    3. Select the transformation which best corresponds to the matrix
    $M = \begin{bmatrix}
        -1/2 & 1/2 \\
        1/2 & 1/2
    \end{bmatrix}$

        - [ ] ![q31.png](img/q31.png)
        - [ ] ![q32.png](img/q32.png)
        - [ ] ![q33.png](img/q33.png)
        - [x] ![q34.png](img/q34.png)

        > ✔️ <span style="color: green;">**Correct**</br>The axes have been rotated, and also flipped here.</span>

    ---

    4. A digital image can be stored by putting lots of coloured pixels at their particular coordinates on a grid.

        If we apply a matrix transformation to the coordinates of each of the pixels in an image, we transform the image as a whole.

        Given a starting image (such as this one of “The Ambassadors” [1533] by Hans Holbein the Younger),

        ![q41.png](img/q41.png)

        which is made up of 400×400 pixels, if we apply the same transformation to each of those 160,000 pixels, the transformed image becomes:

        ![q42.png](img/q42.png)

        Pick a matrix that could correspond to the transformation.

        - [ ] 
        $\begin{bmatrix}
            \sqrt{3}/2 & \sqrt{3}/2 \\
            1/2 & 1/2
        \end{bmatrix}$
        - [ ] 
        $\begin{bmatrix}
            1/2 ^ 0 \\
            -\sqrt{3}/2 & 1/2
        \end{bmatrix}$
        - [x] 
        $\begin{bmatrix}
            \sqrt{3}/2 & -1/2 \\
            1/2 & \sqrt{3}/2
        \end{bmatrix}$
        - [ ] 
        $\begin{bmatrix}
            1/2 & 0 \\
            0 & \sqrt{3}/2
        \end{bmatrix}$

        > ✔️ <span style="color: green;">**Correct**</br>This is a rotation matrix (by 30° anticlockwise).</span>

    ---

    5. At the bottom of the “The Ambassadors”, in the middle of the floor, there is a skull that Holbein has already applied a matrix transformation to!

        To undo the transformation, build a matrix which is firstly a shear in the y direction followed by a scaling in y direction. I.e., multiply the matrices,

        $$M = \begin{bmatrix}
            1 & 0 \\
            0 & 8
        \end{bmatrix}\begin{bmatrix}
            1 & 0 \\
            -1/2 & 1
        \end{bmatrix}
        $$

        ```python
        M = [[1, 0],
             [-4, 8]]
        ```

        > ✔️ <spane style="color: green;">**Correct**</br>Well done.</br>Use your answer in the next question to transform the skull back.</span>

    ---

    6. Use your answer from the previous question to transform the skull back to normal. Change the values of the matrix and press Go! to score on this question.

        You can also use this example to experiment with other matrix transformations. Try some of the ones in this quiz. Have a play!

        ![q6.png](img/q6.png)

        > ✔️ <spane style="color: green;">**Correct**</br>Feel free to use the tool to try out different matrices too.</span>

</details>

---

- <details close><summary><h2>Practice Quiz 2 : Solving linear equations using the inverse matrix</h2></summary>

    ### <span style="color: green;">**Congratulations! You passed!**</span>

    #### **Grade received** <span style="color: green;">100%</span>

    #### **Latest Submission Grade** 100%

    #### **To pass** 80% or higher

    ---

    1. In this quiz, you will practice changing from the standard basis to a basis consisting of orthogonal vectors.
    
        Given vectors $v, b_1, b_2$ all written in the standard basis, what is $v$ in the basis defined by $b_1$ and $b_2$? You are given that $b_1$ and $b_2$ are orthogonal to each other.

        $$v=\begin{bmatrix}
            5 \\
            -1 
        \end{bmatrix},\quad b_1=\begin{bmatrix}
            1 \\
            1
        \end{bmatrix},\quad b_2=\begin{bmatrix}
            1 \\
            -1
        \end{bmatrix}$$

       - [ ] 
       $v_b = \begin{bmatrix}
        -3 \\
        2
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        3 \\
        2
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        3 \\
        -2
       \end{bmatrix}$
       - [x] 
       $v_b = \begin{bmatrix}
        2 \\
        3
       \end{bmatrix}$

        > ✔️ <spane style="color: green;">**Correct**</br>The vector $v$ is projected onto the two vectors $b_1$ and $b_2$.</span>

    ---

    2. Given vectors 

        $$v=\begin{bmatrix}
            10 \\
            -5
        \end{bmatrix},\quad b_1=\begin{bmatrix}
            3 \\
            4
        \end{bmatrix},\quad b_2=\begin{bmatrix}
            4 \\
            -3
        \end{bmatrix}$$

        all written in the standard basis, what is $v$ in the basis defined by $b_1$ and $b_2$? You are given that $b_1$ and $b_2$ are orthogonal to each other.

        - [ ] 
        $v_b = \begin{bmatrix}
        11/5 \\
        2/5
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        -2/5 \\
        11/5
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        2/5 \\
        11/5
       \end{bmatrix}$
       - [x] 
       $v_b = \begin{bmatrix}
        2 \\
        11
       \end{bmatrix}$

        > ✔️ <spane style="color: green;">**Correct**</br>The vector $v$ is projected onto the two vectors $b_1$ and $b_2$.</span>

    ---

    3. Given vectors 

        $$v=\begin{bmatrix}
            2 \\
            2
        \end{bmatrix},\quad b_1=\begin{bmatrix}
            -3 \\
            1
        \end{bmatrix},\quad b_2=\begin{bmatrix}
            1 \\
            3
        \end{bmatrix}$$

        all written in the standard basis, what is $v$ in the basis defined by $b_1$ and $b_2$? You are given that $b_1$ and $b_2$ are orthogonal to each other.

        - [ ] 
        $v_b = \begin{bmatrix}
        -2/5 \\
        5/4
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        -2/5 \\
        4/5
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        5/4 \\
        -5/2
       \end{bmatrix}$
       - [x] 
       $v_b = \begin{bmatrix}
        2/5 \\
        -4/5
       \end{bmatrix}$

        > ✔️ <spane style="color: green;">**Correct**</br>The vector $v$ is projected onto the two vectors $b_1$ and $b_2$.</span>

    ---

    4. Given vectors 

        $$v=\begin{bmatrix}
            1 \\
            1 \\
            1
        \end{bmatrix},\quad b_1=\begin{bmatrix}
            2 \\
            1 \\
            0
        \end{bmatrix},\quad b_2=\begin{bmatrix}
            1 \\
            -2 \\
            -1
        \end{bmatrix},\quad b_3=\begin{bmatrix}
            -1 \\
            2 \\
            -5
        \end{bmatrix}$$

        all written in the standard basis, what is $v$ in the basis defined by $b_1, b_2$ and $b_3$? You are given that $b_1, b_2$ and $b_3$ are orthogonal to each other.

        - [ ] 
        $v_b = \begin{bmatrix}
        3 \\
        -1 \\
        -2
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        -3/5 \\
        -1/3 \\
        -2/15
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        -3/5 \\
        -1/3 \\
        2/15
       \end{bmatrix}$
       - [x] 
       $v_b = \begin{bmatrix}
        3/5 \\
        -1/3 \\
        -2/15
       \end{bmatrix}$

        > ✔️ <spane style="color: green;">**Correct**</br>The vector $v$ is projected onto the two vectors $b_1, b_2$ and $b_3$.</span>

    ---

    5. Given vectors 

        $$v=\begin{bmatrix}
            1 \\
            1 \\
            2 \\
            3
        \end{bmatrix},\quad b_1=\begin{bmatrix}
            1 \\
            0 \\
            0 \\
            0
        \end{bmatrix},\quad b_2=\begin{bmatrix}
            0 \\
            2 \\
            -1 \\
            0
        \end{bmatrix},\quad b_3=\begin{bmatrix}
            0 \\
            1 \\
            2 \\
            0
        \end{bmatrix},\quad b_4=\begin{bmatrix}
            0 \\
            0 \\
            0 \\
            3
        \end{bmatrix}$$

        all written in the standard basis, what is $v$ in the basis defined by $b_1, b_2, b_3$ and $b_4$? You are given that $b_1, b_2, b_3$ and $b_4$ are orthogonal to each other.

        - [ ] 
        $v_b = \begin{bmatrix}
        0 \\
        1 \\
        1 \\
        1
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        1 \\
        0 \\
        1 \\
        1
       \end{bmatrix}$
       - [ ] 
       $v_b = \begin{bmatrix}
        1 \\
        1 \\
        0 \\
        1
       \end{bmatrix}$
       - [x] 
       $v_b = \begin{bmatrix}
        1 \\
        1 \\
        1 \\
        0
       \end{bmatrix}$

        > ✔️ <spane style="color: green;">**Correct**</br>The vector $v$ is projected onto the two vectors $b_1, b_2, b_3$ and $b_4$.</span>

</details>

---

- <details close><summary><h2>Practice Quiz 3 : Linear dependency of a set of vectors</h2></summary>

    ### <span style="color: green;">**Congratulations! You passed!**</span>

    #### **Grade received** <span style="color: green;">83.33%</span>

    #### **Latest Submission Grade** 83.33%

    #### **To pass** 80% or higher

    ---

    1. In the lecture videos you saw that vectors are linearly dependent if it is possible to write one vector as a linear combination of the others. For example, the vectors $a, b$ and $c$ are linearly dependent if $a=q_1b+q_2c$ where $q_1$ and $q_2$ are scalars.

        Are the following vectors linearly dependent?

        $$a=\begin{bmatrix}
            1 \\
            1
        \end{bmatrix},\quad and~~b=\begin{bmatrix}
            2 \\
            2
        \end{bmatrix}$$

       - [x] Yes
       - [ ] No

        > ✔️ <spane style="color: green;">**Correct**</br>When there are two vectors we only need to check if one can be written as a scalar multiple of the other. We can see that the vectors are linearly dependent because $a=\frac{1}{2}b$</span>

    ---

    2. We say that two vectors are linearly independent if they are not linearly dependent, that is, we cannot write one of the vectors as a linear combination of the others. Be careful not to mix the two definitions up!

        Are the following vectors linearly independent?

        $$a=\begin{bmatrix}
            1 \\
            1
        \end{bmatrix},\quad and~~b=\begin{bmatrix}
            2 \\
            1
        \end{bmatrix}$$

       - [x] Yes
       - [ ] No

        > ✔️ <spane style="color: green;">**Correct**</br>These vectors are linearly independent as one is not a scalar multiple of the other.</span>

    ---

    3. We also saw in the lectures that three vectors that lie in the same two dimensional plane must be linearly dependent. This tells us that $a, b$ and $c$ are linearly dependent in the following diagram:

        ![q33.png](img/q33.png)

        What are the values of $q_1$ and $q_2$ that allow us to write $a = q_1b+q_2c$? Put your answer in the following codeblock:

        ```python
        # Assign the correct values for q1 and q2 to write a as a linear combination of b and c
        q1 = -1
        q2 = -3
        ```

        > ✔️ <spane style="color: green;">**Correct**</br>Good job!</span>

    ---

    4. In fact, an $n$-dimensional space can have as many as $n$ linearly independent vectors. The following three vectors are three dimensional, which means that we must check if they are linearly dependent or independent.

        Are the following vectors linearly independent?

        $$a=\begin{bmatrix}
            1 \\
            0 \\
            0
        \end{bmatrix},\quad b=\begin{bmatrix}
            1 \\
            1 \\
            0
        \end{bmatrix},\quad and~~c=\begin{bmatrix}
            1 \\
            0 \\
            1
        \end{bmatrix}$$

       - [x] Yes
       - [ ] No

        > ✔️ <spane style="color: green;">**Correct**</br>These vectors are linearly independent as one can not be written as a linear sum of the other two.</span>

    ---

    5. Are the following vectors linearly independent?

        $$a=\begin{bmatrix}
            1 \\
            0 \\
            1
        \end{bmatrix},\quad b=\begin{bmatrix}
            2 \\
            -1 \\
            1
        \end{bmatrix},\quad and~~c=\begin{bmatrix}
            -3 \\
            1 \\
            -2
        \end{bmatrix}$$

       - [ ] Yes
       - [x] No

        > ✔️ <spane style="color: green;">**Correct**</br>We can that one of the vectors can be written as a linear sum of the other two, $a=-b-c$</span>

    ---

    6. The following set of vectors cannot be used as a basis for a three dimensional space. Why?

        $$a=\begin{bmatrix}
            1 \\
            2 \\
            0
        \end{bmatrix},\quad b=\begin{bmatrix}
            -2 \\
            1 \\
            3
        \end{bmatrix},\quad and~~c=\begin{bmatrix}
            4 \\
            3 \\
            -3
        \end{bmatrix}$$

        - [ ] The vectors are linearly independent.
        - [x] The vectors are not linearly independent.
            > ✔️ <spane style="color: green;">**Correct**</br>We can see that $c = 2a - b$, so the vectors are linearly dependent. The definition of a basis requires that the vectors are linearly independent.</span>
        - [ ] The vectors do not span three dimensional space.
        - [ ] There are too many vectors for a three dimensional basis.
        
        > ✖️ <span style="color: red;">**Incorrect**</br>You didn't select all the correct answers.</span>

</details>

---

## Graded Quiz : Vector operations assessment

### <span style="color: green;">**Congratulations! You passed!**</span>

#### **Grade received** <span style="color: green;">100%</span>

#### **Latest Submission Grade** 100%

#### **To pass** 80% or higher

---

1. In this assessment, you will be tested on all of the different topics you have in covered this module. Good luck!

    A ship travels with velocity given by 
    $\begin{bmatrix}
        1 \\
        2
    \end{bmatrix}$
    , with current flowing in the direction given by 
    $\begin{bmatrix}
        1 \\
        1
    \end{bmatrix}$
    with respect to some co-ordinate axes.

    What is the velocity of the ship in the direction of the current?

    - [ ] 
    $\begin{bmatrix}
        2/3 \\
        2/3
    \end{bmatrix}$
    - [x] 
    $\begin{bmatrix}
        3/2 \\
        3/2
    \end{bmatrix}$
    - [ ] 
    $\begin{bmatrix}
        2/3 \\
        3/2
    \end{bmatrix}$
    - [ ] 
    $\begin{bmatrix}
        3/2 \\
        2/3
    \end{bmatrix}$

    > ✔️ <spane style="color: green;">**Correct**</br>This is the vector projection of the velocity of the ship onto the velocity of the current.</span>

---

2. A ball travels with velocity given by 
$\begin{bmatrix}
    2 \\
    1
\end{bmatrix}$
with wind blowing in the direction given by 
$\begin{bmatrix}
    3 \\
    -4
\end{bmatrix}$
with respect to some co-ordinate axes.

    What is the size of the velocity of the ball in the direction of the wind?

    - [ ] $\frac{5}{2}$
    - [x] $\frac{2}{5}$
    - [ ] $-\frac{2}{5}$
    - [ ] $-\frac{5}{2}$

    > ✔️ <spane style="color: green;">**Correct**</br>This is the scalar projection of the velocity of the ball onto the velocity of the wind.</span>

---

3. Given vectors 
$v=\begin{bmatrix}
    -4 \\
    -3 \\
    8
\end{bmatrix}$,
$b_1=\begin{bmatrix}
    1 \\
    2 \\
    3
\end{bmatrix}$,
$b_2=\begin{bmatrix}
    -2 \\
    1 \\
    0
\end{bmatrix}$, and
$b_3=\begin{bmatrix}
    -3 \\
    -6 \\
    5
\end{bmatrix}$ all written in the standard basis, what is $v$ in the basis defined by $b_1, b_2$ and $b_3$? You are given that $b_1, b_2$ and $b_3$ are all pairwise orthogonal to each other.

    - [x] $\begin{bmatrix}
        1 \\
        1 \\
        1
    \end{bmatrix}$
    - [ ] $\begin{bmatrix}
        0 \\
        1 \\
        1
    \end{bmatrix}$
    - [ ] $\begin{bmatrix}
        1 \\
        0 \\
        1
    \end{bmatrix}$
    - [ ] $\begin{bmatrix}
        1 \\
        1 \\
        0
    \end{bmatrix}$

    > ✔️ <spane style="color: green;">**Correct**</br>This is a change of basis in 3 dimensions.</span>

---

4. Are the following vectors linearly independent?

    $$a=\begin{bmatrix}
        1 \\
        2 \\
        -1
    \end{bmatrix},\quad b=\begin{bmatrix}
        3 \\
        -4 \\
        5
    \end{bmatrix},\quad and~~c=\begin{bmatrix}
        1 \\
        -8 \\
        7
    \end{bmatrix}$$

    - [ ] Yes
    - [x] No

    > ✔️ <spane style="color: green;">**Correct**</br>One can be written as a linear combination of the other two.</span>

---

5. At 12:00 pm, a spaceship is at position $\begin{bmatrix}
    3 \\
    2 \\
    4
\end{bmatrix} km$ away from the origin with respect to some 3 dimensional co ordinate system. The ship is travelling with velocity $\begin{bmatrix}
    -1 \\
    2 \\
    -3
\end{bmatrix} \frac{km}{s}$ What is the location of the spaceship after 2 hours have passed?

    - [ ] $\begin{bmatrix}
        2 \\
        4 \\
        1
    \end{bmatrix}$
    - [x] $\begin{bmatrix}
        1 \\
        6 \\
        -2
    \end{bmatrix}$
    - [ ] $\begin{bmatrix}
        -2 \\
        4 \\
        -1
    \end{bmatrix}$
    - [ ] $\begin{bmatrix}
        -1 \\
        -6 \\
        2
    \end{bmatrix}$

    > ✔️ <spane style="color: green;">**Correct**</br>This takes the idea of vectors in the context of a moving body.</span>
