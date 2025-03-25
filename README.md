# Discrimination-free pricing
A Python implementation of the paper "Discrimination free insurance pricing" 
_Cite: Lindholm, Mathias and Richman, Ronald and Tsanakas, Andreas and Wuthrich, Mario V., Discrimination-Free Insurance Pricing (January 16, 2020). ASTIN Bulletin open access FirstView 2021 https://www.cambridge.org/core/journals/astin-bulletin-journal-of-the-iaa/article/discriminationfree-insurance-pricing/ED25C4053690E56050F437B8DF2AD117, Available at SSRN: https://ssrn.com/abstract=3520676 or http://dx.doi.org/10.2139/ssrn.3520676_

The method from the paper does not depend on the choice of model and its aim is to provide a weighted average price on protected variable.
In the Jupyter Notebook you can find the class and an example with the dataset from Kaggle https://www.kaggle.com/datasets/harishkumardatalab/medical-insurance-price-prediction/data

For many years, laws have required that insurers maintain non-discriminatory pricing policies. This presents a significant challenge, as pricing models often rely on a variety of policyholder characteristics, many of which are correlated with one another. As of a result, protected attributes (e.g. sex, ethnicity) can be inferred from non-protected attributes (e.g., age, smoking habits). To comply with non-discrimination laws, one might initially consider removing protected attributes from the pricing model altogether. However, this approach only addresses direct discrimination. It fails to eliminate indirect discrimination, which occurs when protected characteristics can be 
inferred from other (legitimately used) attributes or when a systematic disadvantage is imposed on a group protected by non-discrimination laws (Tobler, 2008). In this context, the paper “Discrimination-Free Insurance Pricing” by Lindholm et al. (2022) proposes a method to eliminate both direct and indirect discrimination. An implementation of this method is already available in R. However, with the growing popularity of Python in the data science community, its extensive range of models, and the flexibility it offers, having a Python implementation is highly valuable. 

_Cite: Tobler, C. (2008). Limits and potential of the concept of indirect discrimination. Directorate General for Employment, Social Affairs and Equal Opportunities, Unit G2, European Commission. _

**Dataset**: https://www.kaggle.com/datasets/harishkumardatalab/medical-insurance-price-prediction/data
**Method**: In short, the method involves first calculating best-estimate prices for all policyholders. Then, a weighted average price is applied across the protected variable to remove any potential discrimination.
**_Note_**: These methods were specifically chosen to demonstrate that the discrimination-free pricing approach is model agnostic and can be applied across different types of models. 
