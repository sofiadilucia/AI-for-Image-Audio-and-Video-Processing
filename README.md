# Burn Depth Classification Using CNN

Correct assessment of burn depth is a fundamental step in the clinical management of burn injuries, as it directly affects treatment decisions and patient outcomes. In particular, the distinction between superficial burns and deeper injuries is crucial for determining whether surgical intervention, such as skin grafting, is required. However, accurate burn depth evaluation strongly depends on the visual experience of specialized clinicians and is therefore subject to variability and limited availability of expertise. Automated analysis of burn images has the potential to reduce subjectivity, improve early treatment decisions, and limit unnecessary patient transfers.

The present work is inspired by the study *"Segmentation and classification of burn images by color and texture information”*, in which color and texture descriptors extracted from segmented burn regions are used as inputs to a neural network classifier.

While the original approach relies on handcrafted feature extraction and a Fuzzy-ARTMAP neural network, in this notebook we investigate burn depth classification using RGB images and convolutional neural networks. CNNs allow to learn discriminative representations directly from resized color images, potentially reducing the need for manual feature design while preserving sensitivity to color and texture patterns. Due to the limited size of the available dataset, both binary and multiclass classification settings are explored.


**Reference Work**

This work is inspired by the methodology proposed in [Begoña Acha Pinero et al., 2005](https://doi.org/10.1117/1.1921227).
