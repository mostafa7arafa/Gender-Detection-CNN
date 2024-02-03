# Gender Detection CNN Readme

## 1. Introduction

The focus of this project revolves around image processing and pattern recognition. Throughout the term, we delved into various techniques to preprocess datasets containing images and applied diverse classification methods. Our selected dataset centers around gender classification, a task that has gained significance due to the growing capabilities of computers in discerning gender through pictures, voices, or text. While this technology has vast potential applications in security, marketing, and human-computer interaction, it introduces complexities and raises crucial questions related to fairness and privacy.

## 2. Proposed Models

The dataset comprises approximately 27,000 images categorizing only two genders, with around 18,000 for men and 9,000 for women. The images are organized into two folders with equivalent filenames. Our approach involves the development of a handcrafted model.

## 3. Results

### Data Preprocessing Techniques

1. Brightness & contrast
2. Sharpening
3. Removing noise
4. Adjusting image colors in HSV space
5. Resizing and scaling
6. Inverse Transform
7. Histogram equalization
8. Canny Edge Detector

Despite applying eight image enhancement techniques, the accuracy experienced a decline from 91% to 85%. Notably, the accuracy for only four techniques reached 86.6%, and for two techniques, it reached 87.3%. Surprisingly, the dataset did not exhibit a need for enhancement, as applying these filters resulted in a performance degradation. By applying 10 epochs, the accuracy reached 95.27%. The confusion matrix revealed that for the validation set, out of 3536 men images, the model correctly classified 3430 and misclassified 196 entries. For 1901 women images, the model correctly classified 1622 entries and misclassified 276 images.
![image](https://github.com/mostafa7arafa/Gender-Detection-CNN/assets/58299212/7ef229a3-48a2-4f2c-bf6d-ffc5f94d70f0)

## 4. Conclusion

In conclusion, this paper emphasizes the exploration of image quality enhancement through a comprehensive set of techniques. These include adjustments to brightness and contrast, sharpening, noise removal, color adjustment in HSV space, resizing and scaling, inverse transform, histogram equalization, and the utilization of the Canny Edge Detector. However, the findings underscore the significant degradation in model performance after applying these enhancement filters. This underscores the importance of assessing the necessity for image enhancement, as the high-quality images in the dataset were inherently clear to the model, making additional enhancement counterproductive.
