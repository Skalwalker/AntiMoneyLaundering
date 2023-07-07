<a target="_blank" href="https://colab.research.google.com/github/Skalwalker/AntiMoneyLaundering/blob/main/anti_money_laundering.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

# [ALDER](https://github.com/Skalwalker/AntiMoneyLaundering): **A**nti Money **L**aundering using **DE**cision T**R**ees

This project proposes and explores ALDER, an implementation of decision trees and random forest algorithms to detect money laundering. It is designed to classify laundering transactions and can process large-scale data in a simulated distributed environment. ALDER utilizes the IBM Transactions for Anti Money Laundering (IBM TAML) dataset and leverages Apache Spark for scalable computing. It can either use a single decision tree or distribute the computation of multiple decision trees to create a scalable random forest predictor. Therefore, ALDER aims to address research questions related to its effectiveness in classifying money laundering, its performance with different dataset sizes, and its scalability in real distributed environments.

Over many contributions, ALDER applies a rigorous data engineering pipeline with a strong exploratory data analysis. Such combinations allowed ALDER to create robust features able to generalize the content of the data without creating data leakages to potential overfitting. Additionally, ALDER does not rely on external libraries for its decision tree nor its random forest, designing a decision tree from scratch with mechanisms to work with data imbalance, big data thresholds and multiple information gain functions. Finally, ALDER applies a state-of-the-art hyperparameter tuning with Bayesian optimization and the Hyperopt library.

![](https://raw.githubusercontent.com/Skalwalker/AntiMoneyLaundering/main/images/overview.png)
