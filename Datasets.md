
# Datasets for Domain Adaptation


## Cityscape

**Cite**：Marius Cordts, Mohamed Omran, Sebastian Ramos, Timo Rehfeld, Markus Enzweiler, Rodrigo Benenson, Uwe Franke, Stefan Roth, and Bernt Schiele. The cityscapes dataset for semantic urban scene understanding. In CVPR, pages 3213–3223, 2016. 5  

**Download Page**: https://www.cityscapes-dataset.com/

**Introduction**: A real-world dataset for semantic segmentation featuring driving scenes and dense manual annotations. The dataset consists of street view images captured in 50 different cities. 

**Training Set**: 2,975

**Validation Set**: 500

<img src="image-20221019201044630.png" alt="image-20221019201044630" style="zoom:50%;" />



## GTA5

**Cite**: S. R. Richter, V. Vineet, S. Roth, and V. Koltun. Playing for Data: Ground Truth from Computer Games. In European Conference on Computer Vision, 2016. 5  

**Links**: [paper](https://arxiv.org/pdf/1608.02192v1.pdf),  [paper_with_code](https://paperswithcode.com/dataset/gta5), [page/download](https://download.visinf.tu-darmstadt.de/data/from_games/), 

**Introduction**: The datasets consists of 24966 densely labelled frames split into 10 parts for convenience. The class labels are compatible with the [CamVid](http://mi.eng.cam.ac.uk/research/projects/VideoRec/CamVid/) and [CityScapes](https://www.cityscapes-dataset.com/) datasets. We provide sample code for reading the label maps and a split into training/validation/test set [here](https://download.visinf.tu-darmstadt.de/data/from_games/code/read_mapping.zip). Note that a small set of label maps (60 frames) has a different resolution than their corresponding image (thanks to Dequan Wang and Hoang An Le for pointing this out). Please also note that the data is for research and educational use only.

The code for extracting data from games is available here: https://bitbucket.org/visinf/projects-2016-playing-for-data

The datset include 33 different categories.

**Training Set:** We can split the dataset by our need in actually applications. 

**Validataon Set:** The same as we did in the training set.

<img src="image-20221019202137066.png" alt="image-20221019202137066" style="zoom:50%;" />

## SYNTHIA

**Cite:** G. Ros, L. Sellart, J. Materzynska, D. Vazquez, and A. M. Lopez. The SYNTHIA Dataset: A Large Collection of Synthetic Images for Semantic Segmentation of Urban Scenes. In Conference on Computer Vision and Pattern Recognition,
\2016. 6  

**Links:** [paper_with_code](https://paperswithcode.com/dataset/synthia), [page](https://synthia-dataset.net/), [downloads](http://synthia-dataset.net/downloads/)

**Introduction:** The *SYNTHetic collection of Imagery and Annotations*, is a dataset that has been generated with the purpose of aiding semantic segmentation and related scene understanding problems in the context of driving scenarios. SYNTHIA consists of a collection of photo-realistic frames rendered from a virtual city and comes with precise pixel-level semantic annotations for [**13 classes**](http://synthia-dataset.net/table-classes/): misc, sky, building, road, sidewalk, fence, vegetation, pole, car, sign, pedestrian, cyclist, lane-marking.

- 这是一个关于虚拟场景的合成图像数据集。
- 该数据集由来自虚拟城市的 9,400 个多视点照片级真实帧组成，每帧分辨率为 1,280×960，并带有 13 类像素级语义标注，分别为混合场景、天空、建筑物、道路、人行道、围栏、植被、杆、汽车、标志、行人、自行车车手、车道标记。

- 该数据集可用于解决驾驶场景的语义分割和场景理解问题。

- 子集：

  - SYNTHIA-AL，这是以 25 FPS 生成的视频流子集，包含大量地面实况信息。

  - SYNTHIA-SF，这是以 5 FPS 生成的视频序列子集，包含 6 个序列。

  - SYNTHIA-RAND，这是包含原始 13,407 张图像的子集。

  - SYNTHIA-RAND-CITYSCAPES，这是包含 9,400 张随机图像的子集。

  - SYNTHIA VIDEO SEQUENCES，这是以 5 FPS 生成的视频子集，包含 7 个序列。

**Training Set:** We can split the dataset by our need in actually applications. 

**Validataon Set:** The same as we did in the training set.

![image-20221019202937683](image-20221019202937683.png)

## Dark Scences

### Dark Zurich

**Cite:** Christos Sakaridis, Dengxin Dai, and Luc Van Gool. Guided curriculum model adaptation and uncertainty-aware evaluation for semantic nighttime image segmentation. In Int. Conf. Comput. Vis., pages 7374–7383, 2019. 1, 2, 6, 7, 8  

**Links:** [paper_with_code](https://paperswithcode.com/dataset/dark-zurich), [page/downloads](https://www.trace.ethz.ch/publications/2019/GCMA_UIoU/), [code](https://github.com/sakaridis/MGCDA),

**Introduction:** Dark Zurich is an image dataset containing a total of **8,779** images captured at nighttime, twilight, and daytime, along with the respective GPS coordinates of the camera for each image. These GPS annotations are used to construct **cross-time-of-day correspondences**, i.e., to match each nighttime or twilight image to its daytime counterpart.

Zurich dataset also contains another 201 annotated nighttime images including 50 for validation (Dark Zurich-val) and 151 for testing (Dark Zurich-test), for quantitative evaluation. Note that the Dark Zurich-test serves as an online benchmark whose ground truth are not publicly available. 

The Dark Zurich dataset consists of **2,416** nighttime images, **2,920** twilight images and 3,041
daytime images for training, which are all unlabeled with a resolution of **1, 920 × 1, 080.** Images in these three domains can be coarsely aligned by using GPS-based nearest neighbor assignment to compensate the translation in each direction and the zoom in/out factors. 

**Training Set:** We can split the dataset by our need in actually applications. 

**Validataon Set:** The same as we did in the training set.

<img src="image-20221019204125165.png" alt="image-20221019204125165" style="zoom:50%;" />

### Nighttime Driving

**Cite:** Dengxin Dai and Luc Van Gool. Dark model adaptation: Semantic image segmentation from daytime to nighttime. In 2018 21st International Conference on Intelligent Transportation Systems (ITSC), pages 3819–3824. IEEE, 2018. 1, 2, 6, 7 

**Links:** [paper_with_code](https://paperswithcode.com/dataset/nighttime-driving), [page/downloads](http://people.ee.ethz.ch/~daid/NightDriving/#)

**Introduction:** The Nighttime Driving test set contains **50** nighttime images of resolution **1, 920 × 1, 080**
from diverse visual scenes. All these 50 images have been annotated at the pixel level using the same 19 Cityscapes category labels. 

**Training Set:** No open source

**Validation Set:** 50 images.

### ACDC

**Cite:** Christos Sakaridis, Dengxin Dai, and Luc Van Gool. ACDC: The adverse conditions dataset with correspondences for semantic driving scene understanding. In Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV), October 2021. 6, 7, 8  

**Links:** [paper_with_code](https://paperswithcode.com/dataset/acdc-adverse-conditions-dataset-with), [page/downloads](https://acdc.vision.ee.ethz.ch/)

**Introduction:** It contains four adverse-condition categories (fog, rain, snow and nighttime) with pixel-level annotations. Each of them contains **1000** images and is split into train set, validation set and test set for roughly 4:1:5 proportion. The test set is withheld for testing online. 

<img src="image-20221019211342097.png" alt="image-20221019211342097" style="zoom:67%;" />

<img src="image-20221019211719076.png" alt="image-20221019211719076" style="zoom:67%;" />

### NightCity  

**Cite:**

**Links:**

**Introduction:** The NightCity includes **4,297** real night-time images with ground truth pixel-level
semantic annotations. As compared with Cityscapes, NightCity covers more diverse and challenging exposure conditions that are typical in nighttime scenes. 

image size: 1024 * 512  

<img src="image-20221020104932009.png" alt="image-20221020104932009" style="zoom:50%;" />

<img src="image-20221020104854470.png" alt="image-20221020104854470" style="zoom:67%;" />

<img src="image-20221020104751571.png" alt="image-20221020104751571" style="zoom:50%;" />

<img src="image-20221020104811132.png" alt="image-20221020104811132" style="zoom:67%;" />

## Foggy Scences

### Foggy Cityscapes DBF

**Cite:** Christos Sakaridis, Dengxin Dai, and Luc Van Gool. Semantic foggy scene understanding with synthetic data. International Journal of Computer Vision, 126(9):973–992, 2018. 1, 2, 5, 6, 7  

**Links:** [paper_with_code](https://paperswithcode.com/dataset/foggy-cityscapes), [page](http://people.ee.ethz.ch/~csakarid/SFSU_synthetic/), 

**Introduction:** The Foggy Cityscapes has 550 synthetic foggy images in total, including 500training images and 50 testing images. These images are selected from Cityscapes and synthesized with fog using depth information. 

The authors develop a fog simulation pipeline for real outdoor scenes and apply it to the complete set of 25000 images in the Cityscapes dataset to obtain **Foggy Cityscapes**. The authors also define a **refined set** of **550 training+validation Cityscapes images** out of the original 3475 ones, which yield high-quality synthetic fog. The resulting collection of 550 foggy images is termed **Foggy Cityscapes-refined**.

The authors provide three different versions of **Foggy Cityscapes** for the 5000 training+validation+testing Cityscapes images, each characterized by a constant attenuation coefficient which determines the fog density and the visibility range. The values of the attenuation coefficient are 0.005, 0.01 and 0.02m-1 and correspond to visibility ranges of 600, 300 and 150m respectively. For the 20000 extra training Cityscapes images, the authors provide a single version with attenuation coefficient of 0.01m-1. Examples of **Foggy Cityscapes** scenes for varying fog density are shown below.

<img src="image-20221019212655320.png" alt="image-20221019212655320" style="zoom:50%;" />

<img src="image-20221019212118738.png" alt="image-20221019212118738" style="zoom: 50%;" />

<img src="image-20221019212138793.png" alt="image-20221019212138793" style="zoom: 50%;" />

### Foggy Zurich

**Cite:** Christos Sakaridis, Dengxin Dai, Simon Hecker, and Luc Van Gool. Model adaptation with synthetic and real data for semantic dense foggy scene understanding. In ECCV, pages 687–704, 2018. 1, 2, 5, 6, 8  

**Links:** 

**Introduction:** The Foggy Zurich contains **3808 real-world foggy** road scenes, with pixel-level semantic annotations for 16 images with dense fog, in the city of Zurich and its suburbs. According to fog density, it is split into two categories — light and medium, consisting of **1552** **images** and **1498 images**, respectively. Besides, it has a test set–Foggy Zurich-test including 40 images with labels that are compatible with Cityscapes   

<img src="image-20221020100327489.png" alt="image-20221020100327489" style="zoom:50%;" />

### Foggy Driving

**Cite:** Christos Sakaridis, Dengxin Dai, Simon Hecker, and Luc Van Gool. Model adaptation with synthetic and real data for semantic dense foggy scene understanding. In ECCV, pages 687–704, 2018. 1, 2, 5, 6, 8  

**Links:** [paper_with_code](https://paperswithcode.com/dataset/foggy-cityscapes), [page](http://people.ee.ethz.ch/~csakarid/SFSU_synthetic/), 

**Introduction:** The Foggy Driving consists of 101 color images depicting **real-world foggy** driving scenes, in which 33 images are finely annotated and the rest 68 images are coarsely annotated.  51 of these images were captured with a cell phone camera in foggy conditions at various areas of Zurich, and the rest 50 images were collected from the web. The maximum image resolution in the dataset is 960x1280 pixels.

Foggy Driving features pixel-level semantic annotations for the set of 19 classes that are used for evaluation in Cityscapes. Individual instances of the 8 classes from the above set which correspond to humans or vehicles are labeled separately, which affords bounding box annotations for these classes. In total, Foggy Driving contains more than 500 annotated vehicles and almost 300 annotated humans. Given its moderate scale, this dataset is meant for evaluation purposes and we recommend against using its annotations to train semantic segmentation or object detection models. Example images along with their semantic annotations as well as overall annotation statistics are presented below.

They are purely used for **testing**.  

<img src="image-20221019212427463.png" alt="image-20221019212427463" style="zoom: 50%;" />







