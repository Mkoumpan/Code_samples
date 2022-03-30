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

**Execution**

The program can be executed as follows:

-- Upload notebook on Google Colab or run on Jupyters Notebook

**STAR**

Situation: We had to automatically classify thousands of images of people playing musical instruments.

Task: The task was to predict between 12 different classes of people playing musical instruments

Action: We used a a two-stream CNN Deep Learning architecture to model the data. The first stream used pose estimation (mask of the original image with only the pose) and the second the whole image.  The features extracted from the two
CNN streams were then fused to perform the classification process. The advatange of that approach is the extra information the model has about the pose of the person playing the instrument which boosts the classification accuracy by a significant percent.

Solution: We used various classification metrics such as accuracy, F-1 score, confusion matrix to evaluate our results and managed to improve the original model by 5%.


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
