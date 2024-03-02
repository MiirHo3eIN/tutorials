# Vector Quantization 
A vector quantizer maps $R^k$ large dimensional vector into a finite set of vectors, i.e., codewords ($Y$): 


$Y = {y_i : i = 1, 2, 3, ..., N}$ 

where N $<<$ K. 

## Voronoi Region

The nearest neighbor region to each codeword ($Y_i$) is called the Voronoi region and is defined as follows: 

$V_i = {x \in \mathbb{R}^k: || x-y_i|| < || x-Y_j||  \text{for all}  i \neq j }$


where ||.|| is the Euclidean distance between the entry query and the codeword. 

## Similarity Search
Given a set of vectors (codewords) ${x_1, x_2, ..., x_n}$ in dimension $d$, when given a new vector $x$ in dimenstion $d$, the similarty search task finds the minimal distance between query $x$ and codewords: 

$i = argmin_i||x-x_i||$

where ||.|| can be any distance; however, a branch of VQ implementations uses Euclidean distance. 


Computing Euclidean for high dimensional data is a computationally demanding method with a $O(nK)$ complexity. 

The [Product Quantization for Nearest Neighbor Search](https://ieeexplore.ieee.org/abstract/document/5432202) introduces **P**roduct **Q**uantiz (PQ) method, which can be seen as a lossy compression method for high dimensional vectors.    

### Product Quantization for Nearest Neighbor Search 
To Be Aded.



Lately, with emerging era of Neural Networks, in the context of AutoEncoders (AE), Oord et.al.,
