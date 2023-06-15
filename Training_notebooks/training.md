# TRAINING NOTEBOOKS

- Trained multiple U-Net models using the segmentation-models-pytorch.
- Trained models with the backbone 
    1) mit_b2 , mitb3 , mit_b4 , mit_b5
    2) VGG19
    3) resnet50 resnet34
    4) efficientnet_b3
    5) resnest
    6) regnety 
    etc
- Few of them can be found in the repo.
- Trained a model using stratified K fold technique
- During the training the fragments were broken into the sizes of 224 by 224 and kept a stride of 224//4
- trained for 15 epochs by keeping one of the 3 fragments as the cross validation 
- The calculated metric was fbeta score keeping the beta value 0.5
- Was getting the CV score of single model around 63

