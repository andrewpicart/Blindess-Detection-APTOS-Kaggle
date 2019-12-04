# Capstone: Detecting Diabetic Retinopathy

#### Project by: Andrew Picart

## Contents
- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Data](#Data)
- [Conclusion and Recommendations](#Conclusion-and-Recommendations)

## Problem Statement

Diabetic Retinopathy is the leading cause of preventable blindness. According to the National Eye Institute, all forms of diabetic eye disease have the potential to cause severe vision loss and blindness.

The Asia Pacific Tele-Ophthalmology Society ([APTOS](https://www.kaggle.com/c/aptos2019-blindness-detection/overview/aptos-2019)) has sponsored a kaggle competition. The aim is help people with diabetes in rural areas of India with the early detection of diabetic retinopathy. The people in rural areas are at higher risk, since medical screening is difficult to conduct.

With the help of computer-vision models, patients will not have to rely on a skilled doctor to help stop a preventable disease.



## Executive Summary

To aid in the classification of Diabetic Retinopathy, a convolution neural network was created.  The network consists of Conv2D, MaxPooling2D, BathNormalization, and Dense layers in sklearn. There are a total of 2.9 million parameters in the model.  The use of ImageDataGenerator was also used. This allowed for noise to be introduced into the photos and well as apply zoom, crop, and sheer to a random set of photos. This noise helped train the model for a generalized approach when classifying the pictures.



## Data

The dataset was gathered from kaggle.com. The [competition](https://www.kaggle.com/c/aptos2019-blindness-detection/overview) is sponsored by the Asia Pacific Tele-Ophthalmology Society ([APTOS](https://www.kaggle.com/c/aptos2019-blindness-detection/overview/aptos-2019)). APTOS provided the set of 1928 images for training. The images were unaltered from their original collection, some pictures contained artifacts.

Each picture was categorized on a scale from 0-4, with 0 being 'No DR' and 4 being 'Severe DR'. The categories were binarized to have a classification of either 'No DR' or 'DR'. The distribution for the two categories are 50.71% 'No DR' and 49.29% 'DR'.

The full dataset can be found [here](https://www.kaggle.com/c/aptos2019-blindness-detection/data).

## Conclusion and Recommendations

The model performed with an F1 score of 93%. The ROC score was also 93%. While this is a very good metric, I would not be comfortable with deploying the model without further training data. When dealing with people and a condition as permanent as blindness, I would want to have a model that performs even better. I would only recommend using this model for a preliminary screening.

Luckily, there are many other teams working on this project. The community is very helpful and are committed to help solving this issue.
