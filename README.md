# 3D_image_segmentation_via_deep_CNN

### Description:
      - This models were trained for the [kaggle compitition]([url](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/overview)) and won a **BRONZE** medal.
      - Given a fragment, this segmentation model detects the ink.
      - The output of the model is a binary mask where the 1 represents the presence of ink and 0 for no ink.
      - This above mask is then converted into the RLE(Run Length Encodings).
      
### Dataset:
      - The data is taken from the [kaggle compitition](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/data).
      - The dataset is 3d x-ray scans of detached fragments of ancient papyrus scrolls.
      - The training data had 3 fragments.
      - It had the slices from the 3d x-ray surface volume. Each file contains a greyscale slice in the z-direction. Each fragment contains          65 slices. Combined this image stack gives us width * height * 65 number of voxels per fragment.
        ![The 65 channels](https://github.com/Vishak-Bhat30/3D_image_segmentation/assets/102585626/1e48b650-c888-45b4-8930-ab69f8b69b06             "The 65 slices of the first fragment")
        
      - The inklables were given which was a binary mask which showed 1 for the presense of the ink.
       ![inklabels](https://github.com/Vishak-Bhat30/3D_image_segmentation/assets/102585626/8e0f1b70-be98-4a6d-8668-78a551a83545 "labels")

      - Further there was even the mask of the fragment which basically shows where the data is present in the fragment.
      ![mask-bin](https://github.com/Vishak-Bhat30/3D_image_segmentation/assets/102585626/47fa9262-e9c0-4b9d-ba47-157053117633 "mask")



      
