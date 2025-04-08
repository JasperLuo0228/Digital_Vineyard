# Digital Vineyard: Generative Adversarial Network (GAN) Modeling and Feature Analysis Based on Red Wine Quality Dataset
## Overview

This repository contains a machine learning project focused on the application of a Generative Adversarial Network (GAN) to the domain of red wine quality assessment. The code utilizes TensorFlow and Keras for constructing and training the GAN model, which comprises two main components: a generator and a discriminator.

### Data Preprocessing

The dataset is sourced from a publicly available GitHub URL and contains various chemical characteristics of wines alongside quality ratings. The preprocessing steps include:
- Checking and handling missing values.
- Standardizing features using `StandardScaler`.

### Model Architecture

The generator and discriminator networks are built using dense layers, with each having different configurations:
- The generator network includes ReLU activations and batch normalization.
- The discriminator network uses LeakyReLU activations and dropout layers.

### Training Process

- A training function is defined to train the GAN, which includes training the discriminator on real and fake data, followed by the generator.
- Model checkpoints are used to save the model weights at specified intervals.
- The training process is verbose, providing updates on loss and accuracy.

### Post-Training Analysis

- Generated data is created using the trained generator.
- Evaluation metrics like Wasserstein distance and diversity score are computed to assess the quality of the generated data compared to the original dataset.
- Visualizations include pair plots, histograms, and heatmaps to analyze feature distributions and correlations.

### Outlier Detection

- A function is defined to identify outliers in the generated data.
- Outliers are visualized in the pair plots to differentiate between normal data points and anomalies.

### Visualization and Analysis

- Extensive visualizations are created to compare the original and generated data distributions.
- Correlation heatmaps are used to understand feature interactions.
- Box plots and histograms are plotted to inspect the distribution of features across different quality ranges.

### Conclusion

This project demonstrates the capability of GANs to model complex distributions and provides a framework for analyzing the synthetic data in comparison to the real-world data.

### Sources
DateSet - https://www.kaggle.com/code/yldzburhan/predict-wine-quality-factors-lgbm-xgb

Software used - https://www.singlestore.com/spaces/

---

**Keywords:** GAN, Red Wine Quality, TensorFlow, Keras, Data Visualization, Feature Analysis, Outlier Detection.
