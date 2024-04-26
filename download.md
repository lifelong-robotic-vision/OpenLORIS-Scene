# OpenLORIS-Scene Datasets

This page is an index of the [OpenLORIS-Scene](https://lifelong-robotic-vision.github.io/dataset/scene) datasets, and is the only place you can find links to download them. **Please bookmark this page or save the url for future reference.**

## Terms of Use

The OpenLORIS-Scene datasets are released with the [CC BY-ND 4.0](https://creativecommons.org/licenses/by-nd/4.0/) license, which means you can do anything with the data, even for commercial purposes, except distributing derivative datasets (contact us at [openloris@gmail.com](mailto:openloris@gmail.com) if you would like to do so). We would appreciate it if you **cite**[our paper](https://arxiv.org/abs/1911.05603) when appropriate.

## Cite

X Shi, D Li et al. “**Are We Ready for Service Robots? The OpenLORIS-Scene Datasets for Lifelong SLAM**.” arXiv:1911.05603 (2019). [[pdf](https://arxiv.org/pdf/1911.05603)]


```
@inproceedings{shi2019openlorisscene,
    title={Are We Ready for Service Robots? The {OpenLORIS-Scene} Datasets for Lifelong {SLAM}},
    author={Xuesong Shi and Dongjiang Li and Pengpeng Zhao and Qinbin Tian and Yuxin Tian and Qiwei Long and Chunhao Zhu and Jingwei Song and Fei Qiao and Le Song and Yangquan Guo and Zhigang Wang and Yimin Zhang and Baoxing Qin and Wei Yang and Fangshi Wang and Rosa H. M. Chan and Qi She},
    booktitle={2020 International Conference on Robotics and Automation (ICRA)},
    year={2020},
    pages={3139-3145},
}
```

## Contact

The best way to raise any questions or discussions is to open an issue at [lifelong-robotic-vision/OpenLORIS-Scene](https://github.com/lifelong-robotic-vision/OpenLORIS-Scene/issues)

Send us an email only if private discussions are needed (e.g. for talking about collaborations): [openloris@gmail.com](mailto:openloris@gmail.com) 

The market data belong to [Gaussian Robotics](http://www.gs-robot.com/service/vslam/). All other data belong to [iVip of Tsinghua University](http://nics.ee.tsinghua.edu.cn/people/ivip/). The code for collecting and processing the data belong to Intel Corporation. Please contact the corresponding owner if you had any special requests.

## Download

Download files from ***one of*** the following indices of Google Drive, or from [Baidu Pan](https://pan.baidu.com/s/1FoiDFPYPduTEO1CTVRot5g) (code: 59rm). For those who have downloaded package data without groundtruth, check this [groundtruth.zip](https://drive.google.com/file/d/19dz4MhDrhUQp6tIjXv_oQbOmVpsDbHnA/view?usp=sharing) (11 MB).

### New Release of May 2020

**rosbag-all-in-one**: a single compressed* rosbag per trajectory

├── [office1-1_7-rosbag.tar](https://drive.google.com/file/d/1CNEDfHu31RfdUflSfgf3AU0FkkKyTOiP/view?usp=sharing)		7 seq / 225 sec  8.6G	 md5: b55c04...3fdf

├── [corridor1-1_5-rosbag.tar](https://drive.google.com/file/d/1vRu6HcgQDUKp8FwV0k1NICcNwWxQkHbo/view?usp=sharing)	5 seq / 679 sec	25.0G	 md5: 52c1af...f35e

├── [home1-1_5-rosbag.tar](https://drive.google.com/file/d/1t8jsj-x6KnDI8PjuxCg1332cqMvRf9U8/view?usp=sharing)		5 seq / 438 sec	15.3G	 md5: ed81f0...6b12

├── [cafe1-1_2-rosbag.tar		](https://drive.google.com/file/d/1lVhp6Z8GxXFCPd8bR9plHFoVZUadYiBZ/view?usp=sharing)2 seq / 147 sec	 6.3G	 md5: 72fdd0...c18b

└── [market1-1_3-rosbag.tar](https://drive.google.com/file/d/1un6aHylzAJ1nxlaipYcYqgfSxMHsDKkk/view?usp=sharing)**[	](https://drive.google.com/file/d/1lVhp6Z8GxXFCPd8bR9plHFoVZUadYiBZ/view?usp=sharing)3 seq / 755 sec	33.0G	 md5: c3622a...fef3

			         Total: 22 seq /2244 sec / 88G (compressed rosbag**)

\* The bags can be decompressed with [rosbag decompress](http://wiki.ros.org/rosbag/Commandline#decompress) - there is a script in each tar to do that. Decompressed bags would be about 3X larger (284 GB in total). It is possible to play compressed bags directly, but as they would then be decompressed on-the-fly, frame rates may be constrained, depending on your CPU.

** The laser scan data are not available in the market bags. They are packed in separate bags [here](https://drive.google.com/file/d/1JEAs0r071cRCcs3Dw34wXM-xw1LUGgN5/view?usp=sharing). The data were from a 16-beam RS-LIDAR, with a customized message format defined in [ros_rslidar](https://github.com/RoboSense-LiDAR/ros_rslidar). You may need this package to convert the messages into point clouds. For scenes other than market, the laser scan data are available in standard format in the bags above.

**package**: data in png/csv/yaml/etc. which are similar to [TUM format](https://vision.in.tum.de/data/datasets/rgbd-dataset) and can be directly compiled with [SLAMBench](https://github.com/pamela-project/slambench)

├── [office1-1_7-package.tar](https://drive.google.com/file/d/1p_N53AMMjSHY7AlA9xzWv_t2q9R_45uP/view?usp=sharing)		7 seq / 225 sec  9.9G	 md5: 1e5681...890f

├── [corridor1-1_5-package.tar](https://drive.google.com/file/d/1Sy9V7kGM1isIXCbxv9gKvyUc1Zp07jlf/view?usp=sharing)	5 seq / 679 sec	31.3G	 md5: 77cb6d...3695

├── [home1-1_5-package.tar](https://drive.google.com/file/d/1gKv3YgmQHaWiduD8LQrfWUEneK2wlVMu/view?usp=sharing)		5 seq / 438 sec	17.7G	 md5: 7b34bd...c109

├── [cafe1-1_2-package.tar](https://drive.google.com/file/d/1xREhHxxxnX0zxDBTAk_S-XbymSrWFQKD/view?usp=sharing)		2 seq / 147 sec	 7.0G	 md5: d7ac8a...4cb7

└── [market1-1_3-package.tar](https://drive.google.com/file/d/1NjsIg3AXwfF4C_yxtHogu9fst3jkv7rV/view?usp=sharing) 	3 seq / 755 sec	38.8G	 md5: 0a713b...6891

			            Total: 22 seq /2244 sec  105G (compressed with 7z)

\* The laser scan data are not available in the packages.

**Alternative download from Baidu Pan**: [https://pan.baidu.com/s/1FoiDFPYPduTEO1CTVRot5g](https://pan.baidu.com/s/1FoiDFPYPduTEO1CTVRot5g) (code: 59rm) (The files here are a little bit different from those listed above on Google Drive, due to the file size limit of 20GB on Baidu Pan, but their contents are the same.)


---

