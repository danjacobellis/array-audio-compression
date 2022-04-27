# Linear predictive coding

$$s[n] = e[n] + \sum_{k=1}^{P}{a_k s[n-k]}$$

* $s[n]$ is the siganl
* $e[n]$ is the error
* $ \mathbf a = \begin{bmatrix} a_1 & a_2 & \cdots & a_p \end{bmatrix}$ are the parameters
* $ \mathbf r = \begin{bmatrix} r_1 & r_2 & \cdots & r_p \end{bmatrix}$ are the autocorrelation coefficients
* $\mathbf a = \mathbf R ^{-1} \mathbf r$ minimizes $\sum e^2[n]$ 

# Entropy coding

* e[n] modeled as Laplacian
* *Golomb codes* are the optimal prefix code
* Single parameter $M$
* *Rice codes* are suboptimal but force $M$ to be a power of two

# Inter-channel decorrelation

* Map array to *center* and *side* channels

* Make 16 Linear predictions based on the previous 4x4x4 block.

# Lossy compression

* Use mean squared error as distortion function
* Model short segments of audio as Gaussian process

