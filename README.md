# Causality-Inference-XAI

[Youssef ANNAKI](https://www.linkedin.com/in/youssef-annaki-a91ab5192/)

Worked on this research project from June, 2020 to September, 2021 at the Elie Cartan Institute of Lorraine (IECL) and with the collaboration of Inria Paris.

Research done under the supervision of Marianne Clausel (Univ. Lorraine) & Georges Oppenheim (Centre de mathématiques d'Orsay).


## Summary

The aim of this work is to explore more in depth the concept of causality between time series and stochastic processes as well as it inference and to come up with a new approach to this topic.

The research goal relies on our desire to link the world of explainable machine learning with the notion of causality for the analysis of the interaction between time series. More precisely, given a time serie prediction model (regressions, AR models, RNN, ...), we would like to know what are the past events (point in time) of this time serie (or any other time serie used to build the prediction model) that contribute the most to the construction of the prediction. This "contribution" can be seen as causality relationship between past events and predictions. As an example, if we would like to build a stock returns prediction model, we might also be interested in selecting the past price moves / volatility regimes / events that influence the most our prediction process.

To do so, we thought about analysing the concept of causality in a cooperative game theory framework via the Shapley values. This led us to search for the adequate and optimal definition of this values (optimality in terms of mathematical soundnes, statistical estimation and computational time).

This work focuses on the following subjects (non exhaustive):
- Definition and estimation of the linear and non-linear causality (Granger causality, Kernel based Granger causality) for VAR, ARMA, GARCH,... models.

- Sensitivity analysis as a key to the causality concept. We focus on Sobol indices for feature importance quantification in ML regression/prediction tasks and the non-parametric and Monte-Carlo estimation of this indices:

![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/06b84bc0-dd8d-4988-81f8-43f9b451e1d9)

![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/2c922250-1f4d-43a3-9b36-654153069103)

- Linking Shapley values to Sobol indices:

![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/5bac3ad2-5aa6-49be-a597-9dc5429ad112)

- Generalization of the Shapley values to prediction tasks with dependent inputs (features).
- Multi-linear extension of the Shapley values:

![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/4e03a4dc-433f-4a6e-80d7-e1e5fe4bfaef) with 
![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/3422aac9-15aa-4099-ba5c-fb7094d02822)

- Optimal estimation of the Shapley values and optimized parallel computing.
- Time series causality inference on CAC40 high frequency stock price data.

## Some Results

### Linear Granger Causality indice between two time series
![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/70cdd6ba-eded-40ef-9094-bb2a13eeecde)

### Granger Causality graph for {FTSE100, CAC40, S&P500, DAX30}
![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/7238562a-b557-4d2f-b407-04fae503e110)

### Shapley values as a function of the correlation coefficient between 2 features for a gaussian toy model
![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/b9201751-1031-4237-bbd7-16ff6f00fdc0)

### Application of the Shapley values to the explaination of a k-NN prediction model for stock prices
![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/e1769bc6-ff02-4701-a0ed-b510d36e5daf)

### Comparaison fo the Estimation procesdures of the Shapley values
![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/9058ddae-9a7b-44b3-b537-9cac6e512549)

### Estimators' stability analysis
![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/104448d3-65bc-4e77-b6ba-a99ec4537608)

### Rolling window computation/analysis of the shapley values and their change point detection (PELT algorithm) for a given financial time serie
![image](https://github.com/YsfAnnaki/Causality-Inference-XAI/assets/134018406/9f816ba1-7297-4168-a5f8-0aaeefc24e23)



More details regarding the practical convergence rates findings can be found in the project report.

##

For any information, feedback or questions, please [Contact me](mailto:annaki.youssef@gmail.com?subject=[GitHub]%20Source%20Han%20Sans)



