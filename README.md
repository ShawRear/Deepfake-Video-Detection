# Deepfake-Video-Detection
This project is a binary classification project the targets to detect deepfake videos. For this project, I have used _**FaceForensics++(FF++)**_ dataset. The dataset had 1000 original videos sourced from youtube and 5 different kind of manipulated version of those videos making it 5000 in count. 
The preprocessing of the dataset included taking 30 full and still frames from all the videos and then cropping face frames from them. For this task, MTCNN was used.

![Untitled design](https://github.com/user-attachments/assets/b83e37eb-f4eb-4468-9a8f-ccb4e2147f64)

## Model Section
Here comes the split part where images were split into training, testing and validation sets. I used tranformer model Vision Transformer Large (VIT-L) for this project. To adjust the data imbalance issue, I resued the original images of the train set and randomly iterated the manipulated images without replacement to allow the model to learn from the whole dataset. 

![__results___0_1](https://github.com/user-attachments/assets/a55c470d-c42d-4c47-bc5d-3c685403518c)

This is the confusion matrix from the test set.
