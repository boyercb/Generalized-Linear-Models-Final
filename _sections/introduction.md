---
title: "Introduction"
order: 2
---
Principal Component Analysis (PCA) is a common multivariate technique used to reduce a large set of potentially correlated variables into a subset of orthogonal components that maximize the proportion of the variance captured. Originally developed by Karl Pearson to describe the planes of closest fit for a system of points, PCA has since been employed in a number of different disciplines including the construction of wealth indices from asset variables in economics and the classification of phylogenetic species in biology.

More specifically, given an $$n \times p$$ matrix $$\boldsymbol{X}$$, the first principal component is defined as a weighted linear combination of the scaled sample features,

<div>
\begin{aligned}
z = \phi\boldsymbol{X} 
\end{aligned}
</div>

where $$\phi$$ satisfies

<div>
\begin{aligned}
\phi_{(1)} = \textrm{arg max}\left[ \frac{\phi^T\boldsymbol{X}^T\boldsymbol{X}\phi}{\phi^T\phi} \right]
\end{aligned}
</div>

The vector $$\phi$$ is known as the loading vector and the linear combination $$\phi_{(1)}$$ is the first component score. Subsequent components are derived using a similar optimization procedure after removing the previous components. A geometric interpretation of the loading vectors is that they constitute the best $$p$$-dimensional approximation of the column space of $$\boldsymbol{X}$$.
