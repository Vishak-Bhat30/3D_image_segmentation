# 3D_image_segmentation_via_deep_CNN

### Description:

- These models were trained for the [kaggle compitition](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/overview) and won a **BRONZE** medal.
- Given a fragment, this segmentation model detects the ink.
- The output of the model is a binary mask where the 1 represents the presence of ink and 0 for no ink.
- This above mask is then converted into the RLE(Run Length Encodings).


   <img src="https://github.com/Vishak-Bhat30/3D_image_segmentation/assets/102585626/e62e7bd6-71de-43b0-9164-effdec6dd51c" alt="RLE" width="300" />
The following example has the letter "E" it's RLE encoding is: "11 7 20 1 23 1 26 1 29 1 32 1 35 1 38 1 44 1"

 
### Dataset:
- The data is taken from the [kaggle compitition](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/data).
<img src="https://github.com/Vishak-Bhat30/3D_image_segmentation/assets/102585626/c3b0965c-7bbf-4144-9a1d-95532ede7b88" width="200" />

- The dataset is 3d x-ray scans of detached fragments of ancient papyrus scrolls.
- The training data had 3 fragments.
- It had the slices from the 3d x-ray surface volume. Each file contains a greyscale slice in the z-direction. Each fragment contains       65 slices. Combined this image stack gives us width * height * 65 number of voxels per fragment.


  <img src="https://github.com/Vishak-Bhat30/3D_image_segmentation/assets/102585626/1e48b650-c888-45b4-8930-ab69f8b69b06" alt="The 65 channels" width="400" />

  
 The 65 slices of the first fragment
 
- The inklables were given which was a binary mask which showed 1 for the presense of the ink.


  <img src="https://github.com/Vishak-Bhat30/3D_image_segmentation/assets/102585626/8e0f1b70-be98-4a6d-8668-78a551a83545" alt="labels" width="200" />


- Further there was even the mask of the fragment which basically shows where the data is present in the fragment.


  <img src="https://github.com/Vishak-Bhat30/3D_image_segmentation/assets/102585626/47fa9262-e9c0-4b9d-ba47-157053117633" alt="The 65 channels" width="200" />
  
### Contents

- Training_notebooks: Contains the notebooks used for training. Much more description about them is given in the training readme.
- Inference_notebooks: Contains the notebooks used for Inference. Much more description about them is given in the Inference readme.
- tiles_extracted: This is the notebook that reduces the dataset by merging the volume scans with the mask. This removes the 
       unecessary tiles for training the model
