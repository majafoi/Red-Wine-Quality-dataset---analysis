# Red Wine Quality dataset - analysis

Hello, everyone!

In this repository called Red Wine Quality dataset, you can find the code and link to the dataset/data used to make EDA or statistical analysis.

For full code and description, click on the PDF file named Red Wine Qualilty - knitted-exported code from R. 

**SKILL SHOWN - EDA, REGRESSION ANALYSIS, VISUALIZATIONS**

Citation info for the data itself - Citation info: P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis. Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009.; Link - https://archive.ics.uci.edu/ml/datasets/wine+quality

Also, if you tend to use this code, please contact me before you use it, and after permission, make sure to citate me and the citation for the data above. In the PDF file, you can find code extracted/knitted from R Studio, and the explanation written below every graphics. I tried to keep the graphics as simple as possible, but new graphics are incoming in the next PDFs in other repositories.

# Variable names

1. Fixed acidity – most acids involved with wine or fixed or nonvolatile (do not evaporate readily)
2. Volatile acidity – the amount of acetic acid in wine, which at too high of levels can lead to an unpleasant, vinegar taste.
3. Citric acid – found in small quantities, citric acid can add „freshness“ and flavor to wines
4. Residual sugar – the amount of sugar remaining after fermentation stops, it’s rare to find wines with less than 1 g/L and wines with greater than 45g/L are considered sweet
5. Chlorides – the amount of salt in the wine
6. Free sulfur dioxide – the free form of SO2 exists in equilibrium between molecular SO2 (as a dissolved gas) and bisulfite ion; it prevents microbial growth and the oxidation of wine
7. Total sulfur dioxide - amount of free and bound forms of S02; in low concentrations, SO2 is mostly undetectable in wine, but at free SO2 concentrations over 50 ppm, SO2 becomes evident in the nose and taste of wine
8. Density - the density of water is close to that of water depending on the percent alcohol and sugar content
9. ph - describes how acidic or basic a wine is on a scale from 0 (very acidic) to 14 (very basic); most wines are between 3-4 on the pH scale
10. Sulphates - a wine additive which can contribute to sulfur dioxide gas (S02) levels, which acts as an antimicrobial and antioxidant
11. Alcohol - the percent alcohol content of the wine
12. Quality - output variable (based on sensory data, score between 0 and 10)


# Conclusions

After deleting a few extreme outliers, I've come up with the linear model (R2 = 0.2991; p-value < 0.05) that will help calculate the Quality of the red wines in the dataset:

_**Quality = 205,31 + 0,20828 * fixed acidity - 1,04221 * volatile acidity + 0,08765 * residual sugar - 2,04416 * chlorides - 205,35225 * density + 0,89646 * pH + 1,22568 * sulphates**_
