# Dual-Camera-Related

# Table of Contents
- [Optical Flow Estimation](#optical-flow-estimation)
  - [Deep Optical Flow](#deep-optical-flow)
  - [Traditional Optical Flow](#traditional-optical-flow)
  - [Optical Flow Rank](#optical-flow-rank)
- [Stereo Matching](#stereo-matching)
  - [Deep matching](#deep-matching)
  - [Unsupervised Matching](#unsupervised-matching)
- [Flow and Disparity Estimation](flow-and-disparity-estimation)
  - [Deep Flow and Disparity](deep-flow-and-disparity)
  - [Traditional Flow and Disparity](traditional-flow-and-disparity)
- [Datasets](#datasets)
  - [Optical Flow Data](#optical-flow-data)
  - [Matching Data](#matching-data)
- [Leaderboards](#leaderboards)


# Optical Flow Estimation
## Optical Flow Rank
  - ★★★
  - ★★
  - ★
  - ♥
  
## Deep Optical Flow
### **FlowNet**
**[Paper]** FlowNet: Learning Optical Flow with Convolutional Networks <Br>
**[Year]** ICCV 2015 <Br>
**[Author]** Alexey Dosovitskiy, Philipp Fischer, Eddy Ilg, P. Häusser, C. Hazırbaş, V. Golkov, P. Smagt, D. Cremers, Thomas Brox <Br>
**[Pages]** <Br>
https://lmb.informatik.uni-freiburg.de/Publications/2015/DFIB15/ <Br>
**[Description]** <Br>
	
### **FlowNet 2.0**
**[Paper]** FlowNet 2.0: Evolution of Optical Flow Estimation with Deep Networks <Br>
**[Year]** CVPR 2017 <Br>
**[Author]** Eddy Ilg, Nikolaus Mayer, Tonmoy Saikia, Margret Keuper, Alexey Dosovitskiy, Thomas Brox <Br>
**[Pages]** <Br>
https://github.com/lmb-freiburg/flownet2 <Br>
https://github.com/NVIDIA/flownet2-pytorch <Br>
https://lmb.informatik.uni-freiburg.de/resources/software.php <Br>
**[Description]** <Br>
1) FlowNet的改进版, 用了stack等策略. 效果还可以, 但不知在真实数据上的性能有没有保证. <Br>
2) 整篇论文就像一个实验报告, 细节还没研究. <Br>
	
### **SpyNet**
**[Paper]** SPyNet: Spatial Pyramid Network for Optical Flow <Br>
**[Year]** CVPR 2017 <Br>
**[Author]** Anurag Ranjan, [Michael J. Black](https://ps.is.tuebingen.mpg.de/person/black) <Br>
**[Pages]** <Br>
https://github.com/anuragranj/spynet <Br>
**[Description]** <Br>
	
### **PWC-Net**
**[Paper]** PWC-Net: CNNs for Optical Flow Using Pyramid, Warping, and Cost Volum <Br>
**[Year]** CVPR 2018 Oral <Br>
**[Author]** Deqing Sun, [Xiaodong Yang](http://xiaodongyang.org/), [Ming-Yu Liu](http://mingyuliu.net/), [Jan Kautz](http://jankautz.com/) <Br>
**[Pages]** <Br>
https://research.nvidia.com/publication/2018-02_PWC-Net:-CNNs-for <Br>
https://github.com/NVlabs/PWC-Net <Br>
https://github.com/philferriere/tfoptflow <Br>
**[Description]** <Br>	

### **LiteFlowNet**
**[Paper]** LiteFlowNet: A Lightweight Convolutional Neural Network for Optical Flow Estimation <Br>
**[Year]** CVPR 2018 Spotlight <Br>
**[Author]** Tak-Wai Hui, [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[Pages]** <Br>
http://mmlab.ie.cuhk.edu.hk/projects/LiteFlowNet/<Br>
https://github.com/twhui/LiteFlowNet <Br>
**[Description]** <Br>	

**[Paper]** A Lightweight Optical Flow CNN - Revisiting Data Fidelity and Regularization <Br>
**[Year]** TPAMI 2019 <Br>
**[Author]** Tak-Wai Hui, [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[Pages]** <Br>
https://github.com/twhui/LiteFlowNet2 <Br>
**[Description]** <Br>		
	
### **UnFlow**
**[Paper]** UnFlow: Unsupervised Learning of Optical Flow with a Bidirectional Census Loss <Br>
**[Year]** AAAI 2018 <Br>
**[Author]** Simon Meister, Junhwa Hur,  Stefan Roth <Br>
**[Pages]** https://github.com/simonmeister/UnFlow <Br>
**[Description]** <Br>		
	
### **CC**
**[Paper]** Competitive Collaboration: Joint Unsupervised Learning of Depth, Camera Motion, Optical Flow and Motion Segmentation <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  Anurag Ranjan, Varun Jampani,Lukas Balles, [Kihwan Kim](https://www.cc.gatech.edu/~kihwan23/), Deqing Sun, Jonas Wulff , [Michael J. Black](https://ps.is.tuebingen.mpg.de/person/black)<Br>
**[Pages]** <Br>
https://research.nvidia.com/publication/2018-05_Adversarial-Collaboration-Joint <Br>
https://github.com/anuragranj/cc <Br>
**[Description]** <Br>		
  
## Traditional Optical Flow

# Stereo Matching

## Deep Matching

	
### **PSMNet**
**[Paper]** Pyramid Stereo Matching Network<Br>
**[Year]** ECCV 2018 Oral <Br>
**[Author]**  [Jia-Ren Chang](https://jiarenchang.github.io/), [Yong-Sheng Chen](https://people.cs.nctu.edu.tw/~yschen/)<Br>
**[Pages]** <Br>
https://github.com/JiaRenChang/PSMNet <Br>

### **StereoNet**
**[Paper]** StereoNet: Guided Hierarchical Refinement for Real-Time Edge-Aware Depth Prediction<Br>
**[Year]** ECCV 2018 <Br>
**[Author]**  [Sameh Khamis](http://www.samehkhamis.com/), [Sean Fanello](http://www.seanfanello.it/), Christoph Rhemann, Adarsh Kowdle, Julien Valentin, Shahram Izadi<Br>
**[Pages]** <Br>
https://github.com/meteorshowers/StereoNet-ActiveStereoNet <Br>
https://github.com/SPengLiang/StereoNet_Tensorflow <Br>
**[Description]** <Br>	
1) 提出了一个实时的视差估计网络, 分为特征提取, cost volume filtering, refinement三部分, 每部分都使典型的CNN结构. 网络整体结构简单, 速度快(60fps on Titan X), 效果还可以. <Br>
2) 3d Conv还不清楚是怎么用的, 需要之后参考源码.
	
### **MCUA**
**[Paper]** Multi-Level Context Ultra-Aggregation for Stereo Matching <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  [Guang-Yu Nie](https://gy-nie.net/), [Ming-Ming Cheng](https://mmcheng.net/cmm/), [Yun Liu](https://mmcheng.net/yliu/), Zhengfa Liang, [Deng-Ping Fan](http://dpfan.net/), Yue Liu, Yongtian Wang<Br>
**[Pages]** <Br>
http://mmcheng.net/mcua/ <Br>
**[Description]** <Br>	

	
## Unsupervised Matching

### **ActiveStereoNet**
**[Paper]** ActiveStereoNet:End-to-End Self-Supervised Learning for Active Stereo Systems<Br>
**[Year]** ECCV 2018 Oral<Br>
**[Author]** Yinda Zhang, [Sameh Khamis](http://www.samehkhamis.com/), Christoph Rhemann, Julien Valentin, Adarsh Kowdle, Vladimir Tankovich, Michael Schoenberg, Shahram Izadi, Thomas Funkhouser, [Sean Fanello](http://www.seanfanello.it/)<Br>
**[Pages]** <Br>
https://github.com/meteorshowers/StereoNet-ActiveStereoNet <Br>
**[Description]** <Br>	
	
  
# Flow and Disparity Estimation
## Deep Flow and Disparity
### ***Bridging Stereo Matching and Optical Flow***
**[Paper]** Bridging Stereo Matching and Optical Flow via Spatiotemporal Correspondence <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  [Hsueh-Ying Lai](https://lelimite4444.github.io/), [Yi-Hsuan Tsai](https://sites.google.com/site/yihsuantsai/), [Wei-Chen Chiu](https://walonchiu.github.io/)<Br>
**[Pages]** <Br>
https://lelimite4444.github.io/BridgeDepthFlow-Project-Page/ <Br>
**[Description]** <Br>	
1)粗读, 提出了一个将匹配和光流估计结合起来的无监督学习框架. 性能还不错. <Br>

## Traditional Flow and Disparity
### ***Fast Cost-Volume Filtering***
**[Paper]** Fast Cost-Volume Filtering for Visual Correspondence and Beyond <Br>
**[Year]** PAMI 2013 <Br>
**[Author]** Asmaa Hosni, Christoph Rhemann, Michael Bleyer, Carsten Rother, Margrit Gelautz<Br>
**[Pages]** <Br>
https://github.com/fjordyo0707/StereoMatching-CostFilter <Br>
**[Description]** <Br>	
	
# Datasets
## Optical Flow Data
[Sintel](http://sintel.is.tue.mpg.de/)

[Sintel Stereo](http://sintel.is.tue.mpg.de/stereo)

[KITTI Flow](http://www.cvlibs.net/datasets/kitti/eval_scene_flow.php?benchmark=flow)

[UCF 101](https://www.crcv.ucf.edu/data/UCF101.php)

## Matching Data
[KITTI Stereo](http://www.cvlibs.net/datasets/kitti/eval_stereo.php)

[Scene Flow](https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html) <Br>
Paper: A Large Dataset to Train Convolutional Networks for Disparity, Optical Flow, and Scene Flow Estimation


# Leaderboards
[KITTI Flow 2012 Leaderboard](http://www.cvlibs.net/datasets/kitti/eval_stereo_flow.php?benchmark=flow)

[KITTI Flow 2015 Leaderboard](http://www.cvlibs.net/datasets/kitti/eval_scene_flow.php?benchmark=flow)

[KITTI Stereo 2012 Leaderboard](http://www.cvlibs.net/datasets/kitti/eval_stereo_flow.php?benchmark=stereo)

[KITTI Stereo 2015 Leaderboard](http://www.cvlibs.net/datasets/kitti/eval_scene_flow.php?benchmark=stereo)
