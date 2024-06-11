# NeRF Project 
Reconstruct 3D scenes with NeRF and Nerfstudio. 

Project for Fudan University Computer Graphics course, spring 2024. Instructed by Professor [Yan Bo](https://faculty.fudan.edu.cn/yanbo/en/index.htm).

## Demo
Nerfacto model render:
![](assets/demo/nerfacto.gif)

Splatfacto model render:
![](assets/demo/splatfacto.gif)


## Folder Structure
```
NeRF
  |__ assets               
        |__ report            // project report
        |__ slides            // project presentation slides
        |__ demo              // demo GIFs
  |__ dream-gaussian          // dream gaussian notebook & generated 3d model
  |__ eval                    // .json evaluation outputs
  |__ LICENSE 		             
  |__ models                 // trained models
        |__ nerfacto
        |__ splatfacto
  |__ README.md
```

## Dataset 
We first converted and extracted the video frames into images.

Then, we pre-processed 313 images of the M60 tank with COLMAP (feature extraction, feature matching, sparse reconstruction). 
- [Original video of the M60 Tank from Tanks & Temple Dataset](https://www.tanksandtemples.org/download/)
- [COLMAP pre-processed images of the M60 Tank (Kaggle)](https://www.kaggle.com/datasets/jinnywjy/tanks-and-temple-m60-colmap-preprocessed/data)

## Models
We trained and used Nerfstudio's Nerfacto and Splatfacto model. Training was done on Kaggle using the P100 GPU.  
- [Trained Nerfacto model](models/nerfacto/2024-06-07_011037)
- [Trained Splatfacto model](models/splatfacto)
- [Nerfacto training notebook (Kaggle)](https://www.kaggle.com/code/jinnywjy/nerfstudio-nerfacto-model)
- [Splatfacto training notebook (Kaggle)](https://www.kaggle.com/code/jinnywjy/nerfstudio-splatfacto-model)

## Model performance
PSNR (Peak Signal-to-Noise Ratio) is a measure of the peak error between the rendered image and the ground truth image, and it is expressed in decibels (dB). A higher PSNR value indicates better image quality and a closer match to the ground truth image.
| Dataset  | Model | PSNR |
|---|---|---|
| M60 Tank | Nerfacto  | 19.25  |
| M60 Tank  | Splatfacto  | 27.46  |

## Documentation
For more details about the project, please check out our report and presentation slides.
- [Project report (PDF)]()
- [Project presentation slides (PDF)]()

## Extras 
For the extra part of our project, we've decided to build a 3D model and animation of Professor Yan Bo from a 2D image. 

The 3D model was built with DreamGaussian, and the animations were done with Mixamo.

2D image:
![](assets/demo/baseline.png)

Generated 3D model and animation:
![](assets/demo/extra.gif)

## License
Copyright © 2024 JinnyWong, Ng Yu Yue, Zhou Tao, Goh Xin Yie. 

Licensed under the MIT License.

