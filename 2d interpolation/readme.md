# Interpolação 2D e Super-Resolução de Imagens

Este repositório contém uma implementação em Python de múltiplos métodos de interpolação bidimensional, aplicados tanto para dados batimétricos quanto para a super-resolução de imagens, baseado nos algoritmos descritos no artigo:

> **Application of multiple two-dimensional interpolation methods to bathymetric data on the FVCOM unstructured triangular grid**
> Zongli Ruan, Guobing Qian, Yiwei Wang, Jia Xiao
> Applied Mathematics and Computation 507, 129564 (2025)
> DOI: [10.1016/j.amc.2025.129564](https://doi.org/10.1016/j.amc.2025.129564)

O objetivo é replicar os métodos matemáticos de interpolação propostos e validar sua eficácia e eficiência computacional através de tarefas de *Upscaling* (Super-Resolução) de imagens, utilizando métricas quantitativas como PSNR e RRMSE.

## Métodos Implementados

O projeto inclui a implementação vetorizada e otimizada dos seguintes algoritmos:

* **NNI (Nearest Neighbor Interpolation):** Interpolação pelo vizinho mais próximo.
* **Bilinear:** Interpolação linear em direções X e Y.
* **IDW (Inverse Distance Weighting):** Média ponderada pelo inverso da distância ($d^{-2}$).
* **IDWR (Inverse Distance Weighted Regression):** Regressão linear ponderada para correção de suavização local.

## Datasets

Para validação dos algoritmos em cenários de super-resolução, foram utilizados os datasets:

* **Set5**
* **Set14**

Os dados podem ser obtidos em: [Kaggle: Set-5-14 Super Resolution Dataset](https://www.kaggle.com/datasets/ll01dm/set-5-14-super-resolution-dataset)
