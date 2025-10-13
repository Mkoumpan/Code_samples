# TStreamPS: A Two-Stream deep learning method for recognizing human interactions with musical instruments using Pose information in Still images


**Introduction**

Many approaches for action recognition focus on general actions, such as “running” or
“walking”. This work introduces TStreamPS, a method for recognizing interactions
between humans and musical instruments in still images, by utilizing a two-stream
CNN Deep Learning architecture. The first CNN stream of our method consists of
a CNN model that takes as input raw image image pixel information. The second
CNN stream of our architecture takes as input pose information extracted from a
pose estimation tool, in the form of images. The features extracted from the two
CNN streams are then fused to perform the classification process. The experimental
results on the PPMI+ dataset, demonstrate that our method boosted accuracy by
2.33% when compared to a baseline single single stream CNN image classification
architecture, that utilized only appearance information. Also TStreamPS surpassed
the best state-of-the-art method that was evaluated using the PPMI+ dataset by
boosting accuracy by 5.13%.


For further information please read the *TStreamPS_Report.pdf*



## Overview
This project focused on automatically classifying thousands of images of people playing different musical instruments. The goal was to improve recognition accuracy by incorporating pose information alongside the visual appearance of each image through a two-stream deep learning approach.

---

## Situation
We were given a large dataset of images depicting people playing various musical instruments. Manually labeling or analyzing such data was impractical, so an automated classification system was needed to distinguish between 12 instrument classes efficiently and accurately.

---

## Task
The objective was to build a deep learning model capable of classifying each image into one of 12 musical instrument categories. The challenge involved handling visual variability such as different poses, lighting conditions, and instrument orientations.

---

## Action
- **Model Architecture:** Designed and implemented a **two-stream Convolutional Neural Network (CNN)** architecture.  
  - The **first stream** processed pose estimation masks (skeleton representations of the players).  
  - The **second stream** analyzed the full RGB image.  
- **Feature Fusion:** The feature representations extracted from both CNN streams were fused before the classification layer, combining spatial and pose-based information.  
- **Training:** Used data augmentation to improve generalization and trained the model end-to-end using a cross-entropy loss function.  
- **Advantage:** The inclusion of pose information provided contextual cues about player posture and instrument positioning, improving classification robustness.

---

## Result
Evaluation using **accuracy**, **F1-score**, and **confusion matrix** metrics showed a **5% improvement** over the baseline single-stream model.  
The two-stream CNN effectively leveraged pose information to enhance performance, demonstrating the benefit of multi-modal feature fusion in visual classification tasks.

---

## Technologies Used
- **Python**, **TensorFlow / Keras**, **OpenPose** (for pose estimation)
- **NumPy**, **Pandas**, **Matplotlib / Seaborn**
- **CNN architectures** for feature extraction and fusion

**Execution**

The program can be executed as follows:

-- Upload notebook on Google Colab or run on Jupyters Notebook


**References**

[1]Chollet, F.: Xception: Deep learning with depthwise separable convolutions.
CoRR (2016)

[2] Diba, A., Pazandeh, A.M., Pirsiavash, H., Gool, L.V.: Deepcamp: Deep convolutional action attribute mid-level patterns. In: Proc. IEEE Conference on
Computer Vision and Pattern Recognition, pp. 3557–3565. Las Vegas, NV
(2016)

[3] Girshick, R., Donahue, J., Darrell, T., Malik, J.: Rich Feature Hierarchies
for Accurate Object Detection and Semantic Segmentation. In: 2014 IEEE
Conference on Computer Vision and Pattern Recognition, pp. 580–587 (2014)

[4] Gkioxari, G., Girshick, R., Malik, J.: Contextual action recognition with
R*CNN. In: Proc. IEEE International Conference on Computer Vision, pp.
1080–1088. Santiago, Chile (2015)

[5] He, K., Zhang, X., Ren, S., Sun, J.: Deep residual learning for image recognition. CoRR (2015)

[6] He, K., Zhang, X., Ren, S., Sun, J.: Deep residual learning for image recognition. In: Proc. IEEE Conference on Computer Vision and Pattern Recognition,
pp. 770–778. Las Vegas, NV (2016)

**Languages Used**

Python 3.7

**License**

All the code belongs to the University of Houston. Copying and redistribution is not allowed.
