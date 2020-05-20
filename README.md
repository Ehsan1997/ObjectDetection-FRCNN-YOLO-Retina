<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/Ehsan1997/ImageSegmentation-UNET-DeepLab-SegNet">
    <img src="https://coloradoengineering.com/wp-content/uploads/2017/09/Computer-Vision-and-Machine-Learning.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Object Detection Using Deep Learning (Retinanet-YOLO-Faster RCNN)</h3>

  <p align="center">
    Object Detection on Satellite Imagery using various state of the art deep learning techniques. The dataset used is SIMD dataset.
    <br />
    <strong>SIMD Dataset is private »</strong>
    <br />
    <br />
    <a href="https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina/blob/master/FasterRCNN.ipynb">Faster RCNN (Training + Inference)</a>
    ·
    <a href="https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina/blob/master/Retinanet.ipynb">Retina Net (Training + Inference)</a>
    ·
    <a href="https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina/blob/master/YOLO.ipynb">YOLO (Training + Inference)</a>
  </p>
  
  <p align="center">
    <a href="https://drive.google.com/file/d/10G03aobnixPSlKL_1_uEntf629bNukLf/view?usp=sharing">Faster RCNN (Weights Only)</a>
    ·
    <a href="https://drive.google.com/file/d/1-EfuTdqIwqJPTrvmAZ3wSkFyWWmdZvpI/view?usp=sharing">Retina Net (Weights Only)</a>
    ·
    <a href="https://drive.google.com/file/d/1-2jURM9Z6qE8lRELIRBxr1UrnXShhlZc/view?usp=sharing">YOLO (Weights Only)</a>
  </p>
  
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Obtaining Data](#obtaining-data)
* [Usage](#usage)
* [Results](#results)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)
* [Acknowledgements](#acknowledgements)



<!-- ABOUT THE PROJECT -->
## About The Project

[![Sample Image from the dataset][product-screenshot]](https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina)

SIMD Dataset consists of varying sized images taken from google earth and then labelled. These images consist of vehicles and various other objects (only vehicles are labelled). Some techniques are generic and do not resize the input image. Others, like YOLO, require resizing of the image.

### Network Diagrams

_**Network Diagrams are too large to be plotted, summary of networks is shown with keras's model.summary method.**_

#### Faster RCNN
![Faster RCNN Architecture](https://www.researchgate.net/profile/Vysakh_Mohan2/publication/330822827/figure/fig1/AS:727572925145090@1550478311441/This-image-shows-the-Faster-RCNN-Pipeline-Initial-layers-are-convolutional-layers-of.png)

#### Retina Net
![Retina Net Architecture](https://www.researchgate.net/publication/329817799/figure/fig7/AS:706118477156352@1545363172094/One-step-RetinaNet-architecture-in-prediction-mode-from-full-image-input-to-detection.png)

#### YOLO
![YOLO Architecture](https://www.researchgate.net/publication/335865923/figure/fig1/AS:804106595758082@1568725360777/Structure-detail-of-YOLOv3It-uses-Darknet-53-as-the-backbone-network-and-uses-three.jpg)

### Built With
Major Libraries that were used in this project,
* [Keras](https://keras.io)
* [Tensorflow](https://tensorflow.org)
* [Numpy](https://numpy.org)



<!-- GETTING STARTED -->
## Getting Started

The notebooks provided in this repository are standalone and can be run directly using colab.

### Prerequisites

Account on colab is recommended, although not required.

### Obtaining Data

Data is private and cannot be obtained through any public channel. Only people from SEECS NUST may acquire this data.



<!-- USAGE EXAMPLES -->
## Usage

There are weights for each model available, although these weights are used in the notebooks after training.

In order to download the respective model weights, use the links provided at the start of this readme.

If you have to use the weights with your own model, then just upload the desired model weights to the workspace and run the notebook.

### Config File
Most of the configuration were already present in the repositories from which the implementation of the required techniques was used.

## Results

### Training Settings

Different Hyperparameters were used for the training. Approximately 100 epochs, learning rate of 1e-5 and batch size of 1 was used.

### Quantitative Results
| Model | Training Loss | Validation mAP | Test mAP |
| ------------- | ------------- | ------------- | ------------- |
| Faster RCNN | 1.18 | 18.04 | 21.01 |
| Retinanet | 0.6 | 68.03 | 65.3 |
| YOLO | 19.60 | 54.1 | 53.7 |



#### *For each model, (i)Qualitative Results (ii)Training and Validation graphs are shown.*

### Qualitative Results

#### Faster RCNN
![FRCNN Visual Results][frcnn-qual-res]
#### Retina Net
![RetinaNet Visual Results][retinanet-qual-res]
#### YOLO
![YOLO][yolo-qual-res]

### Training and Validation Graphs

#### Faster RCNN
![FRCNN Training Loss][frcnn-train-graph]
#### Retina Net
![Retina Net Training Loss][retinanet-train-graph]
#### YOLO
![YOLO Training Loss][yolo-train-graph]

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/Ehsan1997/ImageSegmentation-UNET-DeepLab-SegNet/issues) for a list of proposed features (and known issues).



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Muhammad Ehsan ul Haq - [@EhsanBinEjaz](https://twitter.com/EhsanBinEjaz) - ehsanulhaq18@gmail.com

Project Link: [https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina](https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [Faster RCNN Implementation by kbardool](https://github.com/kbardool/keras-frcnn)
* [Retina Net Implementation by fizyr](https://github.com/fizyr/keras-retinanet)
* [YOLO v3 Implementation by experiencor](https://github.com/experiencor/keras-yolo3)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Img Shields](https://shields.io)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Pages](https://pages.github.com)
* [Animate.css](https://daneden.github.io/animate.css)
* [Loaders.css](https://connoratherton.com/loaders)
* [Slick Carousel](https://kenwheeler.github.io/slick)
* [Smooth Scroll](https://github.com/cferdinandi/smooth-scroll)
* [Sticky Kit](http://leafo.net/sticky-kit)
* [JVectorMap](http://jvectormap.com)
* [Font Awesome](https://fontawesome.com)





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina.svg?style=flat-square
[contributors-url]: https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina.svg?style=flat-square
[forks-url]: https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina/network/members
[stars-shield]: https://img.shields.io/github/stars/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina.svg?style=flat-square
[stars-url]: https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina/stargazers
[issues-shield]: https://img.shields.io/github/issues/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina.svg?style=flat-square
[issues-url]: https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=flat-square
[license-url]: https://github.com/Ehsan1997/ObjectDetection-FRCNN-YOLO-Retina/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/ehsansonofejaz
[product-screenshot]: readme-images/0014.jpg
[frcnn-train-graph]: unet-train-graph.png
[retinanet-train-graph]: readme-images/retina_graph.png
[yolo-train-graph]: deeplabv3+-train-graph.png
[frcnn-qual-res]: readme-images/frcnn.png
[retinanet-qual-res]: readme-images/retina.png
[yolo-qual-res]: readme-images/yolo.jpg
