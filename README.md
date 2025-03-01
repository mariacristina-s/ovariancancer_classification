# Ovarian Cancer Subtype Classification in histopatological images

This project focuses on the classification of ovarian cancer subtypes using deep learning models applied to histopathological images. The project explores convolutional neural network (CNN) architectures, including ResNet-50, to evaluate the performance in identifying five primary ovarian cancer subtypes:
- High-Grade Serous Carcinoma (HGSC)
- Clear-Cell Ovarian Carcinoma (CC)
- Endometrioid Carcinoma (EC)
- Low-Grade Serous Carcinoma (LGSC)
- Mucinous Carcinoma (MC)

The project involves multiple classification scenarios:
- Binary Classification - Differentiating between two subtypes (EC vs. CC) to establish baseline model performance
- Three-Class Classification - Extending classification to three subtypes (EC, CC, and MC) to analyze multi-class generalization
- Five-Class Classification - Evaluating model performance on all five ovarian cancer subtypes to assess scalability and robustness

The implementation uses TensorFlow and Keras, with data preprocessing including image resizing, normalization, and augmentation techniques to enhance model generalization. The training was done on Google Colab utilizing NVIDIA A100 GPUs, and hyperparameters such as learning rate, batch size, and dropout rates were fine-tuned to optimize performance.

Model performance was assessed using key evaluation metrics, including accuracy, precision, recall, F1-score, and confusion matrices to understand classification errors.

Some findings:

- ResNet-50 achieved high accuracy (97%) in binary classification but showed performance degradation in multi-class scenarios
- Multi-class classification (5 classes) had the lowest accuracy (88%), mainly due to data imbalance and similar morphological characteristics among certain subtypes

Link to dataset here https://www.kaggle.com/competitions/UBC-OCEAN

Credits for dataset to:

(1) Asadi-Aghbolaghi, M.; Farahani, H.; Zhang, A.; Akbari, A.; Kim, S.; Chow, A.; Dane, S.; Consortium, O. C.; Consortium, O.; Huntsman, D. G.; Gilks, C. B.; Ramus, S.; Köbel, M.; Karnezis, A. N.; Bashashati, A. Machine Learning-Driven Histotype Diagnosis of Ovarian Carcinoma: Insights from the OCEAN AI Challenge. medRxiv2024. https://doi.org/10.1101/2024.04.19.24306099.

(2) Farahani, H.; Boschman, J.; Farnell, D.; Darbandsari, A.; Zhang, A.; Ahmadvand, P.; Jones, S. J.; Huntsman, D.; Köbel, M.; Gilks, C. B.; Singh, N.; Bashashati, A. Deep Learning-Based Histotype Diagnosis of Ovarian Carcinoma Whole-Slide Pathology Images. Modern Pathology 2022, 35 (12), 1983–1990.
