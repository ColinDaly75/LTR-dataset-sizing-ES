# Leaning to Rank Dataset Sizing for Enterprise Search

Learning curve graphs can be employed to estimate the required size of a dataset size.   As the dataset size increases, the performance initially increases until the model saturates.  The minimum sufficient dataset size occurs when adding more data does not lead to a significant increase in the performance.   When the model performance saturates, we can potentially assume that the general population and the training dataset now have very similar underlying distributions. Thus, the cost of further computation and storage has diminishing rewards.

![fig-dataset-size-determination](https://github.com/ColinDaly75/LTR-dataset-sizing-ES/assets/51714656/12deb2f8-390e-4b4c-bc74-2245f969311e)


The figure is a learning curve that plots nDCG performance for various training dataset sizes.  The plot is designed to estimate the dataset size required for a target performance value.
The plot shows the ranking performance growing according to a power law and then reaches a plateau.  As the size of training data (number of QD-Pairs) increases, the ranking performance improves following a power law.  But, after about 1000 QD-Pairs, the ranking performance plateaus.   This would suggest that the size of ENTRP-SRCH dataset (2554 QD-Pairs) is more than sufficient and is not a limiting factor.  For reproducibility purposes, the code used to generate this plot is available online\footnote{\href{https://github.com/ColinDaly75/LTR-dataset-sizing-ES}{https://github.com/ColinDaly75/LTR-dataset-sizing-ES}}.  
