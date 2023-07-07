<a target="_blank" href="https://colab.research.google.com/github/Skalwalker/AntiMoneyLaundering/blob/main/anti_money_laundering.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

# [ALDER](https://github.com/Skalwalker/AntiMoneyLaundering): **A**nti Money **L**aundering using **DE**cision T**R**ees

This project proposes and explores ALDER, an implementation of decision trees and random forest algorithms to detect money laundering. It is designed to classify laundering transactions and can process large-scale data in a simulated distributed environment. ALDER utilizes the IBM Transactions for Anti Money Laundering (IBM TAML) dataset and leverages Apache Spark for scalable computing. It can either use a single decision tree or distribute the computation of multiple decision trees to create a scalable random forest predictor. Therefore, ALDER aims to address research questions related to its effectiveness in classifying money laundering, its performance with different dataset sizes, and its scalability in real distributed environments.

Over many contributions, ALDER applies a rigorous data engineering pipeline with a strong exploratory data analysis. Such combinations allowed ALDER to create robust features able to generalize the content of the data without creating data leakages to potential overfitting. Additionally, ALDER does not rely on external libraries for its decision tree nor its random forest, designing a decision tree from scratch with mechanisms to work with data imbalance, big data thresholds and multiple information gain functions. Finally, ALDER applies a state-of-the-art hyperparameter tuning with Bayesian optimization and the Hyperopt library.

![](https://raw.githubusercontent.com/Skalwalker/AntiMoneyLaundering/main/images/overview.png)

## About

This project is a partial requisite for completing the courses of "Algorithms for massive datasets" and "Statistical methods for ML" on the masters degree computer science program from Università degli Studi di Milano.

- **Author:** Renato Avellar Nobre
- **Matriculation Number:** 984405
- **Exam Project Year:** 22/23

### Disclaimer

"I declare that this material, which I now submit for assessment, is entirely my own work and has not been taken from the work of others, save and to the extent that such work has been cited and acknowledged within the text of my work. I understand that plagiarism, collusion, and copying are grave and serious offences in the university and accept the penalties that would be imposed should I engage in plagiarism, collusion or copying. This assignment, or any part of it, has not been previously submitted by me or any other person for assessment on this or any other course of study."
