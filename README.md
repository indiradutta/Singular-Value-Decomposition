# Singular Value Decomposititon
<br>
The singular value decomposition of a matrix A is the factorization of A into the product of three matrices A = UDV^(T) where the columns of U and V are orthonormal and the matrix D is diagonal with positive real entries. The diagonal entries Sigma or S are known as the singular values of M. The number of non-zero singular values is equal to the rank of M. The columns of U and the columns of V are called the left-singular vectors and right-singular vectors of M, respectively.
<br>
It can also be thought of as a study of a matrix by studying it's most fundamental components like it's eigen vectors with an added advantage that the matrix need not be a sqaure matrix unlike PCA.
<br>
## Matrices U, V and S
<br> * The matrix U is the eigen vector matrix of A^(T)A.
     <br>
     * The matrix V is the eigen vector matrix of AA^(T).
     <br>
     * The matrix S is a rectangular diagonal matrix with it's diagonal elements as the square root of the eigen values of U or V (both of them have the same eigen values) also          termed as the singular values of matrix A.
     <br>
## Application of SVD - Image Compression
<br>
SVD has it's use varying across a wide variety of domains. Here, we are using it for Image Compression. Image compression with SVD is a frequently occurring application of this method. The image is treated as a matrix of pixels with corresponding color values and is decomposed into smaller ranks that retain only the essential information that comprises the image. 
The method of image compression with singular value decomposition is based on the idea that if the SVD is known, some of the singular values σ are significant while the others are small and not significant. Thus, if the significant values are kept and the small values are discarded then only the columns of U and V corresponding to the singular values are used.
As we increase the rank, the quality of the image increases.
