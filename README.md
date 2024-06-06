# NeRF Project 
Reconstruct 3D scenes with NeRF and Nerfstudio. 

Project for Fudan University Computer Graphics course, spring 2024. Instructed by Professor [Yan Bo](https://faculty.fudan.edu.cn/yanbo/en/index.htm).

## Demo
- [Rendered M60 Tank video (YouTube)]()


## Folder Structure
```
NeRF
  |__ assets               
        |__ report            // project report
        |__ slides            // project presentation slides
        |__ demo              // demo images and GIFs 
  |__ LICENSE 		           
  |__ models                // trained models
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
- [Trained Nerfacto model]()
- [Trained Splatfacto model]()
- [Nerfacto training notebook (Kaggle)]()
- [Splatfacto training notebook (Kaggle)]()

Model performace:
| Dataset  | Model | PSNR |
|---|---|---|
| M60 Tank | Nerfacto  |   |
| M60 Tank  | Splatfacto  |   |

## Documentation
For more details about the project, please check out our report and presentation slides.
- [Project report (PDF)]()
- [Project presentation slides (PDF)]()

## Extras 



## License
Copyright © 2024 JinnyWong, Ng Yu Yue. 

Licensed under the MIT License.

