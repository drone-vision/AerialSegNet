# AerialSegNet
A deep learning based architecture developed towards UAV-image-based semantic segmentation tasks

## Article in brief
The proposed end-to-end convolutional neural network (CNN) architecture consists of contracting and symmetric expanding paths that precisely extract the global features to segment the vegetation class from the aerial image. The proposed architecture is evaluated on the two UAV image datasets: Urban Drone Dataset (UDD) and NITRDrone Dataset. It succeeds to achieve an intersection over union (IoU) of  and  on the UDD and NITRDrone datasets, respectively, thus demonstrating better performance accuracy than the state-of-the-art methods. The experimentally obtained results show that implementing the dense connections helps to significantly reduce the number of trainable parameters and improves the model’s efficacy in addressing such multi-class segmentation problems, particularly in vegetation detection and road-line extraction.

## Proposed Approach
<p align="center">
 <img src="https://github.com/drone-vision/AerialSegNet/blob/main/images/L_D_UNet_2.png" width=\textwidth " />
 </p>

## Experimental Results

The experimentations are conducted on **NITRDD** dataset and **UDD** dataset. 
The results are as follows:
-NITRDD
| Models  | #Parameters  | mPrecision | mRecall | mIoU | mFScore | mAccuracy |
|---------|--------------|------------|---------|------|---------|-----------|
|FCN-8s   |   136*M*     | 0.58       |0.35     | 0.12 |  0.14   | 0.55      |
|FCN-16s   |  134*M*     |0.81        |0.83     |0.76  |0.81     | 0.95      |
|FCN-32s   |  134*M*     |0.80        |0.82     | 0.71 |0.76     |0.93       |
|FCDenseNet|   9.42*M*   | 0.81       |0.79     | 0.68 |  0.74   | 0.90      |
|SegNet    |  29.44*M*     |0.84        |0.74     |0.68  |0.76     | 0.92      |
|DeepLab_V3+Exception   |  41.3*M* |0.84| 0.79    |0.74  |0.83     | 0.96      |
|UNet-ResNet-18s|  15.50*M*|0.84        |0.90     | 0.80 |0.85     |0.98       |
|UNet-ResNet-50s|  36.49*M*|0.85        |0.90     | 0.81 |0.87     |0.98       |
|**AerialSegNet**|  11.76*M*|0.88       |0.91     | 0.84 |0.88     |0.98       |
                                                                                                           
- \* Update on **UDD** and the executable code will be available soon (A reader can find the results in the base paper)
- The full version of the article can be viewed at "https://www.sciencedirect.com/science/article/pii/S0168169922004112#s0025"
                                                                                                           
## Citation & Acknowledgements

 If this work looks helpful to you don't forget to cite:

    @article{behera2022vegetation,
       title={Vegetation Extraction from UAV-based Aerial Images through Deep Learning},
       author={Behera, Tanmay Kumar and Bakshi, Sambit and Sa, Pankaj Kumar},
       journal={Computers and Electronics in Agriculture},
       volume={198},
       pages={107094},
       year={2022},
       publisher={Elsevier},
       note = "doi: 10.1016/j.compag.2022.107094"
       }
