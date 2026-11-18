---
permalink: /thesis/
title: ""
---

# Context-Aware Anomaly Detection for Complex and Dynamic Industrial Settings

> Check out my thesis [online](https://lirias.kuleuven.be/4452974?&lang=en)! 

The explosion of Internet of Things (IoT) applications has significantly increased the availability of sequential data across virtually any domain in engineering and science, including industry, finance, environmental sciences, astronomy, and healthcare monitoring. This has led to massive collections of time series data, i.e., ordered sequences of observations measuring how one or more variables evolve over time. Given the scale of these collections, manual inspection is no longer feasible, and automated solutions have become a necessity.

In this thesis, we focus on time series anomaly detection: the automatic identification of observations or events that deviate from regular patterns and do not conform to a well-defined notion of normal behaviour. Such anomalies can signal critical events, such as heart failures in cardiology, defects in jet turbine engineering, or ecosystem disturbances in earth sciences. Due to its practical importance, anomaly detection has been thoroughly investigated over the past five decades.

Despite this intensive research, detecting contextual anomalies, observations that are anomalous only with respect to a specific context, remains a significant open challenge. Nevertheless,  context is necessary to accurately detect anomalies in real-world applications, where ``normality'' heavily relies on context. What constitutes an anomaly in one context may be considered normal in another. 

This dissertation investigates context-aware anomaly detection, a general methodology for injecting contextual information into anomaly detection models in an unsupervised manner. To this end, we define context as a partition of the feature space, a formulation that generalises over all existing interpretations of the concept. We then tackle context-aware anomaly detection from two complementary angles: the temporal context, a partition of the time domain into intervals of semantically meaningful behaviour, and the subspace context, a partition of the variable space into subsets of related attributes.

For the temporal context, we propose PaTSS, a novel unsupervised method for time series semantic segmentation that explicitly models gradual state transitions between contexts. Building on this, SemSegAD leverages the identified temporal contexts to perform anomaly detection within each context independently, thereby lifting any existing anomaly detection model into a contextual setting without requiring additional supervision. We demonstrate that SemSegAD not only significantly outperforms existing contextual anomaly detection methods, but also consistently improves upon the performance of the underlying model.

For the subspace context, we propose SubTSMD, a novel method for discovering motifs across variable-size subspaces of a multivariate time series, thereby identifying which groups of variables collectively define a meaningful context. Building on this, HydraAD exploits subspace structure through competing random convolutional kernels to achieve exceptionally fast and accurate anomaly detection.