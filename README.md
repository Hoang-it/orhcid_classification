# Orhcid Classification

The architecture of the model is as follows:
![alt text](https://github.com/Hoang-it/orhcid_classification/image/architecture.jpg?raw=true)

It include 2 part:
1. Segmentation orchid flower (SOF): detects and segments orchid flowers in image
2. Classifier orchid’s species (COS): classifies orchid flowers to its label

This is the result of our model:
|Dataset|mAP|Weights|
|-------|---|-------|
|[Orchid Flowers Dataset][1]
|[Orchid Flowers Classification][2]|


## Segmentation orchid flower (SOF)

It is trained by fine tune the [yolact](https://github.com/dbolya/yolact) model

Yolact paper: https://arxiv.org/abs/1904.02689

The result of SOF is here:
|Dataset|mAP|Weights|
|-------|---|-------|
|[Orchid Flowers Dataset][1]
|[Orchid Flowers Classification][2]|

## Classifier orchid’s species (COS)

Based on idea of this [paper](https://www.researchgate.net/publication/330528310_Efficient_Deep_Features_Selections_and_Classification_for_Flower_Species_Recognition)

We extend it by increase the number of model it use to implement features extraction and change the algorithm it use to select features. This is the result of COS:
|Dataset|mAP|Weights|
|-------|---|-------|
|[Orchid Flowers Dataset][1]
|[Orchid Flowers Classification][2]|

[1]: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/0HNECY
[2]: https://ieee-dataport.org/keywords/orchid-flower-classification
