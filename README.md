# Melanoma Detection
In cancer, there are over 200 different forms. Out of 200, melanoma is the deadliest form of skin cancer. The diagnostic procedure for melanoma starts with clinical screening, followed by dermoscopic analysis and histopathological examination. Melanoma skin cancer is highly curable if it gets identified at the early stages. The first step of Melanoma skin cancer diagnosis is to conduct a visual examination of the skin's affected area. Dermatologists take the dermatoscopic images of the skin lesions by the high-speed camera, which have an accuracy of 65-80% in the melanoma diagnosis without any additional technical support. With further visual examination by cancer treatment specialists and dermatoscopic images, the overall prediction rate of melanoma diagnosis raised to 75-84% accuracy. The project aims to build an automated classification system based on image processing techniques to classify skin cancer using skin lesions images.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- **Motivation** - The overarching goal is to support the efforts to reduce the death caused by skin cancer. The primary motivation that drives the project is to use the advanced image classification technology for the well-being of the people. Computer vision has made good progress in machine learning and deep learning that are scalable across domains.
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
- To overcome the issue of class imbalance, used a python package  Augmentor (https://augmentor.readthedocs.io/en/master/) to add more samples across all classes so that none of the classes have very few samples.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- tensorflow - version 2.17.0
- numpy - version 1.26.4
- pandas - version 2.1.4
- keras - version 3.4.1
- augmentor - version 0.2.12

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Due to the inadequate data in the provided images across different classes, the validation accuracy went down
- After using the python package augmentor for rebalancing the classes in the dataset, the validation accuracy boosted up and hence helped to train the model efficiently
- After augumentation for class rebalancing, the validation accuracy has improved significantly by getting rid of underfitting, but since the training accuracy increased significantly to 93.9%, which is about 13% more that validations accuracy(80.7%).
- There is slight chances of model getting overfitted.
- Autotuning the model helped greatly to maintain the parallelism in the model building process and hence increased the speed of CNN model building with different set of layers.
- Class rebalancing through augumentation helped greatly to identify the significant pattern in the data that model could learn effectively.
- Still validation loss could have been minimized to more better. Increasing the augument data sample could have helped to reduce the val_loss little mode.

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- Melanoma Skin Cancer from https://www.cancer.org/cancer/melanoma-skin-cancer/about/what-is-melanoma.html
- Upgrad for providing the guidance to understand the CNN architecture and its practical application

## Contact
Created by [@anantjs11] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
