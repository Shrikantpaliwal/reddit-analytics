This software package gives scalable implementation of Neighbor Embedding (NE), which is a set of nonlinear dimensionality reducion algoirthms that recently developed for data visualization.

You may need to re-compile the C/C++ codes by running "compile_ne(2)" or "compile_ne(3)". The former is for 2D visualizations and the latter is for 3D.

The main entrance function is "ne_wrapper". Type 'help ne_wrapper' for more information.

There are some shortcuts that call the wrapper by default settings, such as "sne_p", "ssne_p", "tsne_p", "nerv_p" and "wtsne_p". Type 'help FUNCTION_NAME' for more information.

The script "demo.m" demonstrates the several example of using the package. Run "compile_ne(2)" before doing the demo.

The function "ne_wrapper" and its shortcuts take a nonnegative symmetric matrix as input. To visualize vectorial data, one can use "x2p" to get the similaries for small datasets. For large datasets, one may first use "fast_knn" and then symmetrize the resulting kNN graph adjacency matrix.


If you use the package in your publishable work, please cite the following papers:

Zhirong Yang, Jaakko Peltonen and Samuel Kaski. Scalable Optimization of Neighbor Embedding for Visualization. In International Conference on Machine Learning (ICML2013), pages 127-135, Atlanta, USA, 2013.

Zhirong Yang, Jaakko Peltonen and Samuel Kaski. Optimization Equivalence of Divergences Improves Neighbor Embedding. In International Conference on Machine Learning (ICML2014), pages 460-468, Beijing, China 2014.

Zhirong Yang, Jaakko Peltonen and Samuel Kaski. Majorization-Minimization for Manifold Embedding. In the 18th International Conference on Artificial Intelligence and Statistics (AISTATS 2015), pages 1088-1097, San Diego, USA 2015.



Zhirong Yang (23-June-2016)
