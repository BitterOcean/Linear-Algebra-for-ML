# Mathematics for Machine Learning: Linear Algebra

**by** Imperial College London

**Taught by**: <a href="https://www.coursera.org/instructor/david-dye">David Due</a>

**Student**: <a href="https://maryamsaeedmehr.github.io/">Maryam Saeidmehr</a>

## About this Course

In this course on Linear Algebra we look at what linear algebra is and how it relates to vectors and matrices. Then we look through what vectors and matrices are and how to work with them, including the knotty problem of eigenvalues and eigenvectors, and how to use these to solve problems. Finally  we look at how to use these to do fun things with datasets - like how to rotate images of faces and how to extract eigenvectors to look at how the Pagerank algorithm works.
Since we're aiming at data-driven applications, we'll be implementing some of these ideas in code, not just on pencil and paper. Towards the end of the course, you'll write code blocks and encounter Jupyter notebooks in Python, but don't worry, these will be quite short, focussed on the concepts, and will guide you through if you’ve not coded before.

At the end of this course you will have an intuitive understanding of vectors and matrices that will help you bridge the gap into linear algebra problems, and how to apply these concepts to machine learning.

| Item | Description |
|---|---|
| 📓 Basic Info  |  Course 1 of 3 in the <a href="https://www.coursera.org/specializations/mathematics-machine-learning">Mathematics for Machine Learning Specialization</a>  |
| ⚖️ Level  | Beginner  |
| ⏰ Commitment  | 5 weeks of study, 2-5 hours/week  |
| 🔤 Language  | English, **Subtitles**: Chinese (Traditional), Arabic, French, Ukrainian, Portuguese (European), Chinese (Simplified), Italian, Portuguese (Brazilian), Vietnamese, Korean, German, Russian, Turkish, Spanish, Japanese</br> <a href="https://www.coursera.org/learn/neural-networks-deep-learning/home/info#">Volunteer to translate subtitles for this course</a>  |
| :wrench: Hardware Req | No additional hardware is needed to complete this course |
| 🧑‍🎓 How To Pass  |  Pass all graded assignments to complete the course. |
| ⭐ User Ratings  | ![Rating](https://img.shields.io/badge/rating-4.7-brightgreen) |

## Syllabus

- <details open><summary><h2>Week 1</h2></summary>

  ### Introduction to Linear Algebra and to Mathematics for Machine Learning

  In this first module we look at how linear algebra is relevant to machine learning and data science. Then we'll wind up the module with an initial introduction to vectors. Throughout, we're focussing on developing your mathematical intuition, not of crunching through algebra or doing long pen-and-paper examples. For many of these operations, there are callable functions in Python that can do the adding up - the point is to appreciate what they do and how they work so that, when things go wrong or there are special cases, you can understand why and what to do.

  <details>
    <summary>📂 5 videos, 4 readings, 3 practice quizzes</summary>

  - Video: Introduction: Solving data science challenges with mathematics
  - Reading: About Imperial College & the team
  - Reading: How to be successful in this course
  - Reading: Grading policy
  - Reading: Additional readings & helpful references
  - Discussion Prompt: Nice to meet you!
  - Ungraded Plugin: Complete our short pre-course survey
  - Video: Motivations for linear algebra
  - Video: Getting a handle on vectors
  - Practice Quiz: Exploring parameter space
  - Practice Quiz: Solving some simultaneous equations
  - Video: Operations with vectors
  - Practice Quiz: Doing some vector operations
  - Video: Summary

  </details>

</details>

---  

- <details open><summary><h2>Week 2</h2></summary>

  ### Vectors are objects that move around space

  In this module, we look at operations we can do with vectors - finding the modulus (size), angle between vectors (dot or inner product) and projections of one vector onto another. We can then examine how the entries describing a vector will depend on what vectors we use to define the axes - the basis. That will then let us determine whether a proposed set of basis vectors are what's called 'linearly independent.' This will complete our examination of vectors, allowing us to move on to matrices in module 3 and then start to solve linear algebra problems.

  <details>
    <summary>📂 8 videos, 3 practice quizzes</summary>

    - Video: Introduction to module 2 - Vectors
    - Video: Modulus & inner product
    - Video: Cosine & dot product
    - Video: Projection
    - Practice Quiz: Dot product of vectors
    - Video: Changing basis
    - Practice Quiz: Changing basis
    - Video: Basis, vector space, and linear independence
    - Video: Applications of changing basis
    - Practice Quiz: Linear dependency of a set of vectors
    - Video: Summary

  </details>

  🔬**Graded**: Vector operations assessment

</details>

---

- <details open><summary><h2>Week 3</h2></summary>

  ### Object Detection

  Apply your new knowledge of CNNs to one of the hottest (and most challenging!) fields in computer vision: object detection.

  <details>
    <summary>📂 8 videos, 2 practice quizzes</summary>

    - Video: Matrices, vectors, and solving simultaneous equation problems
    - Video: How matrices transform space
    - Video: Types of matrix transformation
    - Video: Composition or combination of matrix transformations
    - Practice Quiz: Using matrices to make transformations
    - Video: Solving the apples and bananas problem: Gaussian elimination
    - Video: Going from Gaussian elimination to finding the inverse matrix
    - Practice Quiz: Solving linear equations using the inverse matrix
    - Video: Determinants and inverses
    - Ungraded Lab: Identifying special matrices
    - Video: Summary

  </details>

  🔬**Graded**: Identifying special matrices
  
</details>

---

- <details open><summary><h2>Week 4</h2></summary>

  ### Matrices make linear mappings

  In Module 4, we continue our discussion of matrices; first we think about how to code up matrix multiplication and matrix operations using the Einstein Summation Convention, which is a widely used notation in more advanced linear algebra courses. Then, we look at how matrices can transform a description of a vector from one basis (set of axes) to another. This will allow us to, for example, figure out how to apply a reflection to an image and manipulate images. We'll also look at how to construct a convenient basis vector set in order to do such transformations. Then, we'll write some code to do these transformations and apply this work computationally.

  <details>
    <summary>📂 6 videos, 2 practice quizzes</summary>

    - Video: Introduction: Einstein summation convention and the symmetry of the dot product
    - Practice Quiz: Non-square matrix multiplication
    - Practice Quiz: Example: Using non-square matrices to do a projection
    - Video: Matrices changing basis
    - Video: Doing a transformation in a changed basis
    - Video: Orthogonal matrices
    - Video: The Gram–Schmidt process
    - Ungraded Lab: Gram-Schmidt process
    - Video: Example: Reflecting in a plane
    - Ungraded Lab: Reflecting Bear

  </details>

  🔬**Graded**: Gram-Schmidt Process

  🔬**Graded**: Reflecting Bear

</details>

---

- <details open><summary><h2>Week 5</h2></summary>

  ### Eigenvalues and Eigenvectors: Application to Data Problems

  Eigenvectors are particular vectors that are unrotated by a transformation matrix, and eigenvalues are the amount by which the eigenvectors are stretched. These special 'eigen-things' are very useful in linear algebra and will let us examine Google's famous PageRank algorithm for presenting web search results. Then we'll apply this in code, which will wrap up the course.

  <details>
    <summary>📂 9 videos, 1 reading, 3 practice quizzes</summary>

    - Video: Welcome to module 5
    - Video: What are eigenvalues and eigenvectors?
    - Practice Quiz: Selecting eigenvectors by inspection
    - Video: Special eigen-cases
    - Video: Calculating eigenvectors
    - Practice Quiz: Characteristic polynomials, eigenvalues and eigenvectors
    - Video: Changing to the eigenbasis
    - Video: Eigenbasis example
    - Practice Quiz: Diagonalisation and applications
    - Ungraded Plugin: Visualising Matrices and Eigen
    - Video: Introduction to PageRank
    - Ungraded Lab: PageRank
    - Video: Summary
    - Video: Wrap up of this linear algebra course
    - Reading: Did you like the course? Let us know!
    - Ungraded Plugin: Post-Course Survey

  </details>

  🔬**Graded**: Page Rank

  🔬**Graded**: Eigenvalues and eigenvectors

</details>

## Certificate
  
![Screenshot from 2023-08-15 18-52-05](https://github.com/BitterOcean/Linear-Algebra-for-ML/assets/60509979/a9e87727-c569-4b2d-a3ab-a81ec532c4f8)
  
- ![IssuingOrganization](https://img.shields.io/badge/Issuing%20Organization-Coursera-informational)

- ![IssueDate](https://img.shields.io/badge/Issue%20Date-August%2015,%202023-informational)

- ![CredentialID](https://img.shields.io/badge/Credential%20ID-DCJXL39LMDU6-informational)

- <a href="https://www.coursera.org/account/accomplishments/verify/DCJXL39LMDU6">![CredentialLink](https://img.shields.io/badge/Credential%20Link-https://www.coursera.org/account/accomplishments/verify/DCJXL39LMDU6-informational)</a>

- <a href="https://github.com/BitterOcean/Linear-Algebra-for-ML/blob/main/Coursera%20DCJXL39LMDU6.pdf">![CertificateDownload](https://img.shields.io/badge/Certificate-Download%20PDF-informational)</a>
