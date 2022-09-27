# Automatic Detction of Regional Wall Motion Abnormality from Echocardiogram
Purpose: The echocardiogram is an ultrasound imaging modality,employed to assess cardiac abnormalities. The Regional Wall Motion Abnormality (RWMA) is the occurrence of abnormal or absent contractility of a region of the heart muscle. Conventional assessment of RWMA is based on visual interpretation of endocardial excursion and myocardial thickening from the echocardiogram videos. Wall motion assessment accuracy depends on the experience of the sonographer. Current automated methods highly depend on the preprocessing steps such as segmentation of ventricle part or manually finding systole and diastole frames from an echocardiogram. Additionally, state-of-the-art methods majorly make use of images rather than videos, which specifically lack the usage of temporal information associated with an echocardiogram. The deep learning models used, employ highly complex networks with billions of trainable parameters. Further, the existing models used on video data add to the computational intensity because of the high frame rates of echocardiogram videos.<br />
Methods: We developed a novel deep learning architecture EC3DNet (Echo-Cardio 3D Net), which captures the temporal information for identifying regional wall motion abnormality from Echocardiogram. We demonstrate that EC3D-Net can extract temporal information from even raw echocardiogram videos, at low frame rates, employing minimal training parameter-based deep architecture.<br />
Results: EC3D-Net achieves both an overall F1-Score and an Area Under Curve (AUC) score of 0.82. Further, we were able to reduce time for training and trainable parameters by 50% through minimizing frames per second. We also show the EC3D-Net is an interpretable model, thereby helping physicians understand our model prediction.<br />
Conclusion: RWMA detection from echocardiogram videos is a challenging process and our results demonstrate that we could achieve the state-of-the-art results even while using minimal parameters and time by our EC3D-Net. The proposed network outperforms both complex deep networks as well as fusion methods generally used in video classification.<br />

This study used the HMC-QU dataset. Original dataset available at https://www.kaggle.com/datasets/aysendegerli/hmcqu-dataset <br />
Lower fps data available at https://github.com/SanjeeviGunasekaran/Regional-Wall-Motion-Abnormality-Detection/tree/main/Data

The EC3D-Net Setup <br />
<img src="{{https://github.com/SanjeeviGunasekaran/Automatic-RWMA-Detection/blob/main/overall%20ec3d-net.jpg}}" style="display: block; margin: auto;" />

The EC3D-Net Layers Architecture<br /> 
![plot](https://github.com/SanjeeviGunasekaran/Regional-Wall-Motion-Abnormality-Detection/blob/main/new%20cnn3.jpg)

Interpretability of the EC3D-Net<br /> 
![plot](https://github.com/SanjeeviGunasekaran/Automatic-RWMA-Detection/blob/main/grad%20cam%20image.png)
