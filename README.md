# Deep learning Smartphone Application for Real-Time Detection of Defects in Buildings.

Condition assessment and health monitoring (CAHM) of built assets, require effective and continuous monitoring of any changes to the material and/or geometric properties of the asset in order to detect any early signs of defects or damage and act on time. Most of the traditional CAHM techniques, however, depend on manual labour despite that, in some cases, the inspection environment can be unsafe and could lead to low efficiency or miss-judgement of the severity of the defect. In recent years, computer vision techniques have been proposed as an automated alternative to the traditional CAHM techniques as methods for extracting and analysing feature-related information from asset images and videos. Such methods have proven to be robust and effective solutions, complementary to current time-consuming and unreliable manual observational practices. This work is concerned with the development of a deep learning-based smartphone App which allows real-time detection of 4 types of defects in buildings namely; cracks, mould, stain, and paint deterioration. Since smartphones are widely available and equipped with high-resolution cameras, this application can offer a practical, low-cost solution for condition assessment procedures of built assets.

### The Proposed Detector
A study by Google Research for testing the speed and accuracy of many pre-trained neural network models suggests that SSD with MobileNet is one the fastest and most accurate models for mobile device applications (43). SSD MobileNet is developed in Tensorflow and require a relatively small CPU/GPU loads and low memory consumption whilst maintaining high accuracy. Moreover, SSD MobileNet is particularly optimised for fast run time on embedded devices (such as smartphones) since these networks combine the use of single feed-forward deep neural networks and the architecture of MobileNets. The main distinctive feature of MobileNets is in the deployment of the so-called depthwise separable filters for building the core layers. These filters factorize a full-size convolution into a smaller 1×1 depthwise convolution called pointwise convolution as illustrated in Figure 2 (60).

![ssd](https://user-images.githubusercontent.com/76107657/118638748-10a08280-b7cf-11eb-89dc-07bf4dd50c9e.png)


### Training Dataset

![datasetsample](https://user-images.githubusercontent.com/76107657/118629683-be0e9880-b7c5-11eb-9f4f-68c74df39347.png)

### Augmentation
Data Augmentation
To improve the training experience, all images in the dataset were placed at the centre of a random background image of size 300 x 300 as illustrated by Figure 4. These random background images were obtained from The Visual Geometry Group – University of Oxford. The purpose of adding these random backgrounds is to avoid overfitting yet make the model more robust to various input object shapes and sizes. This is called image manipulation, otherwise data augmentation, a well-known technique in deep learning used to enhance the quality and the size of the training dataset. Data augmentation also include other techniques including such as geometric transformations, colour space augmentations, kernel filters, mixing images, random erasing, amongst others 

![ag](https://user-images.githubusercontent.com/76107657/118639057-64ab6700-b7cf-11eb-810e-424adc0467dd.png)


### Detection Results
![mobile_results](https://user-images.githubusercontent.com/76107657/118629972-01690700-b7c6-11eb-8076-6b0556df6357.png)

Screenshots representing predicted defects obtained from running the smartphone App. (a) represents the detection of cracks with the corresponding accuracy and inference time, (b) represents the detection of paint deterioration with its corresponding accuracy and inference time, (c) represents the detection of mould with its corresponding accuracy and inference time, and finally (d) represents the detection of stain with its corresponding accuracy and inference time.
![mb](https://user-images.githubusercontent.com/76107657/118639525-e8655380-b7cf-11eb-8651-e36512a2d713.png)
![mb4](https://user-images.githubusercontent.com/76107657/118639625-0468f500-b7d0-11eb-9104-121a224d1e61.png)
![mb3](https://user-images.githubusercontent.com/76107657/118639632-059a2200-b7d0-11eb-81d1-3f54ed34da70.png)
![mb2](https://user-images.githubusercontent.com/76107657/118639637-0632b880-b7d0-11eb-9371-a0989eae0915.png)

