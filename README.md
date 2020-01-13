# Two-frame Stereo Correspondence 

# Table of Contents
- [Optical Flow Estimation](#optical-flow-estimation)
  - [Deep Optical Flow](#deep-optical-flow)
  - [Traditional Optical Flow](#traditional-optical-flow)
  - [Unsupervised Optical Flow](#unsupervised-optical-flow)
  - [Optical Flow Rank](#optical-flow-rank)
- [Stereo Matching](#stereo-matching)
  - [Deep matching](#deep-matching)
  - [Traditional Matching](#traditional-matching)
  - [Unsupervised Matching](#unsupervised-matching)
- [Flow And Disparity](#flow-and-disparity)
  - [Deep Flow And Disparity](#deep-flow-and-disparity)
  - [Traditional Flow And Disparity](#traditional-flow-and-disparity)
- [Datasets](#datasets)
- [Leaderboards](#leaderboards)
- [Projects](#projects)


# Optical Flow Estimation
## Optical Flow Rank
  - ★★★
  - ★★
  - ★
  - ♥
  
## Deep Optical Flow
### **FlowNet ★★☆**
**[Paper]** FlowNet: Learning Optical Flow with Convolutional Networks <Br>
**[Year]** ICCV 2015 <Br>
**[Author]** Alexey Dosovitskiy, Philipp Fischer, Eddy Ilg, P. Häusser, C. Hazırbaş, V. Golkov, P. Smagt, D. Cremers, Thomas Brox <Br>
**[Pages]** <Br>
https://lmb.informatik.uni-freiburg.de/Publications/2015/DFIB15/ <Br>
**[Description]** <Br>
	
### **FlowNet 2.0 ★**
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
	
### **PWC-Net ★★**
**[Paper]** PWC-Net: CNNs for Optical Flow Using Pyramid, Warping, and Cost Volum <Br>
**[Year]** CVPR 2018 Oral <Br>
**[Author]** Deqing Sun, [Xiaodong Yang](http://xiaodongyang.org/), [Ming-Yu Liu](http://mingyuliu.net/), [Jan Kautz](http://jankautz.com/) <Br>
**[Pages]** <Br>
https://research.nvidia.com/publication/2018-02_PWC-Net:-CNNs-for <Br>
https://github.com/NVlabs/PWC-Net <Br>
https://github.com/philferriere/tfoptflow <Br>
**[Description]** <Br>	

### **LiteFlowNet ★☆**
**[Paper]** LiteFlowNet: A Lightweight Convolutional Neural Network for Optical Flow Estimation <Br>
**[Year]** CVPR 2018 Spotlight <Br>
**[Author]** Tak-Wai Hui, [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[Pages]** <Br>
http://mmlab.ie.cuhk.edu.hk/projects/LiteFlowNet/<Br>
https://github.com/twhui/LiteFlowNet <Br>
**[Description]** <Br>	
1) 粗读。轻量级光流估计网络，效果和速度都不错. <Br>
2) 采用encoder-decoder结构，逐级估计光流+warp，每个level估计光流时设计了matching+refine两阶段结构. <Br>
3) 另外提出了一个flow regularization策略，对预测的光流进行滤波，其中滤波的kernel是通过网络学习出来的. 感觉作用类似于一个边缘保持滤波器. <Br>

**[Paper]** A Lightweight Optical Flow CNN - Revisiting Data Fidelity and Regularization <Br>
**[Year]** TPAMI 2019 <Br>
**[Author]** Tak-Wai Hui, [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[Pages]** <Br>
https://github.com/twhui/LiteFlowNet2 <Br>
**[Description]** <Br>		
	
  
## Traditional Optical Flow
### ***Optical Flow Filter***
**[Paper]** A Filter Formulation for Computing Real Time Optical Flow <Br>
**[Year]** RAL 2016 <Br>
**[Author]** [Juan David Adarve](http://jadarve.github.io/), David J. Austin, [Robert Mahony](https://users.cecs.anu.edu.au/~Robert.Mahony/) <Br>
**[Pages]** https://github.com/jadarve/optical-flow-filter <Br>
**[Description]** <Br>

### **DIS**
**[Paper]** Fast Optical Flow using Dense Inverse Search  <Br>
**[Year]** CVPR 2016 <Br>
**[Author]** Till Kroeger, [Radu Timofte](http://www.vision.ee.ethz.ch/~timofter/), [Dengxin Dai](http://www.vision.ee.ethz.ch/~daid/), Luc Van Gool <Br>
**[Pages]** https://github.com/tikroeger/OF_DIS <Br>
**[Description]** <Br>

### **BriefMatch**
**[Paper]** BriefMatch: Dense binary feature matching for real-time optical flow estimation  <Br>
**[Year]** SCIA17 <Br>
**[Author]** [Gabriel Eilertsen](http://vcl.itn.liu.se/members/gabriel-eilertsen), Per-Erik Forssén, [Jonas Unger](http://vcl.itn.liu.se/members/jonas-unger) <Br>
**[Pages]** https://github.com/gabrieleilertsen/briefmatch <Br>
**[Description]** <Br>
	
## Unsupervised Optical Flow
### **Unsupervised Flownet ★**
**[Paper]** Back to basics: Unsupervised learning of optical flow via brightness constancy and motion smoothness <Br>
**[Year]** ECCV 2016 Workshops<Br>
**[Author]** [Jason J. Yu](https://www.eecs.yorku.ca/~jjyu/), [Adam W. Harley](http://www.cs.cmu.edu/~aharley/), [Konstantinos G. Derpanis](http://www.scs.ryerson.ca/~kosta/) <Br>
**[Pages]**  <Br>
https://www.eecs.yorku.ca/~jjyu/projects/unsupflow/ <Br>
https://github.com/ryersonvisionlab/unsupFlownet/ (TF) <Br>
**[Description]** <Br>

### ***Unsupervised convolutional neural networks for motion estimation***
**[Paper]** Unsupervised convolutional neural networks for motion estimation <Br>
**[Year]** ICIP 2016<Br>
**[Author]** Aria Ahmadi, Ioannis Patras <Br>
**[Pages]**  <Br>
**[Description]** <Br>
	
### ***Learning Features by Watching Objects Move***
**[Paper]** Learning Features by Watching Objects Move <Br>
**[Year]** CVPR 2017 <Br>
**[Author]** [Deepak Pathak](https://people.eecs.berkeley.edu/~pathak/), [Ross Girshick](http://www.rossgirshick.info/), [Piotr Dollár](https://pdollar.github.io/), [Trevor Darrell](https://people.eecs.berkeley.edu/~trevor/), [Bharath Hariharan](http://home.bharathh.info/) <Br>
**[Pages]**  <Br>
https://people.eecs.berkeley.edu/~pathak/unsupervised_video/ <Br>
**[Description]** <Br>
	
### **UnFlow ★**
**[Paper]** UnFlow: Unsupervised Learning of Optical Flow with a Bidirectional Census Loss <Br>
**[Year]** AAAI 2018 <Br>
**[Author]** Simon Meister, Junhwa Hur,  Stefan Roth <Br>
**[Pages]** https://github.com/simonmeister/UnFlow <Br>
**[Description]** <Br>

			
### **CC ★★**
**[Paper]** Competitive Collaboration: Joint Unsupervised Learning of Depth, Camera Motion, Optical Flow and Motion Segmentation <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  Anurag Ranjan, Varun Jampani,Lukas Balles, [Kihwan Kim](https://www.cc.gatech.edu/~kihwan23/), Deqing Sun, Jonas Wulff , [Michael J. Black](https://ps.is.tuebingen.mpg.de/person/black)<Br>
**[Pages]** <Br>
https://research.nvidia.com/publication/2018-05_Adversarial-Collaboration-Joint <Br>
https://github.com/anuragranj/cc <Br>
**[Description]** <Br>	
1) 大致浏览, 提出一种非监督的联合估计深度, 相机姿态, 光流以及运动物体分割的框架. 用类似于EM的交替迭代优化策略, 利用任务间的相互制约关系提升每个子任务的性能. <Br>
2) 相机姿态和深度的估计适用于静态区域, 光流估计适用于动态区域, 它们之间是竞争关系, motion segmentation用来充当仲裁者的角色. <Br>
3) 从思路和结果来看感觉这篇文章很有趣, 不过不太适用于当前需求, 以后有需要可以深入了解下. <Br>

### **SelFlow ★**
**[Paper]** SelFlow: Self-Supervised Learning of Optical Flow <Br>
**[Year]** CVPR 2019 Oral <Br>
**[Author]**   [Pengpeng liu](https://ppliuboy.github.io/), [Michael R. Lyu](http://www.cse.cuhk.edu.hk/lyu/), [Irwin King](https://www.cse.cuhk.edu.hk/irwin.king/), [Jia Xu](http://pages.cs.wisc.edu/~jiaxu/index.html)<Br>
**[Pages]** <Br>
https://github.com/ppliuboy/SelFlow <Br>
**[Description]** <Br>	

### ***Robustness Meets Deep Learning: An End-to-End Hybrid Pipeline for Unsupervised Learning of Egomotion***
**[Paper]** Unsupervised Event-based Learning of Optical Flow, Depth, and Egomotion<Br>
**[Year]** arXiv 1812 <Br>
**[Author]**  [Alex Zihao Zhu](https://fling.seas.upenn.edu), Wenxin Liu, Ziyun Wang, Vijay Kumar, [Kostas Daniilidis](https://www.cis.upenn.edu/~kostas/)
<Br>
**[Pages]** <Br>
**[Description]** <Br>	
	
### ***Unsupervised Event-based Learning of Optical Flow, Depth, and Egomotion***
**[Paper]** Unsupervised Event-based Learning of Optical Flow, Depth, and Egomotion<Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  [Alex Zihao Zhu](https://fling.seas.upenn.edu), Liangzhe Yuan, Kenneth Chaney, [Kostas Daniilidis](https://www.cis.upenn.edu/~kostas/)
<Br>
**[Pages]** <Br>
**[Description]** <Br>	
	
# Stereo Matching

## Deep Matching

### **SGM-Nets**
**[Paper]** SGM-Nets: Semi-Global Matching With Neural Networks<Br>
**[Year]** CVPR 2017 Oral<Br>
**[Author]** Akihito Seki, [Marc Pollefeys](https://inf.ethz.ch/personal/pomarc/)<Br>
**[Pages]** <Br>
**[Description]** <Br>	
	
### **GCNet ★☆**
**[Paper]** End-To-End Learning of Geometry and Context for Deep Stereo Regression<Br>
**[Year]** ICCV 2017 Oral<Br>
**[Author]** [Alex Kendall](https://alexgkendall.com/), Hayk Martirosyan, [Saumitro Dasgupta](https://ai.stanford.edu/~saumitro/), Peter Henry, Ryan Kennedy, Abraham Bachrach, Adam Bry<Br>
**[Pages]** <Br>
https://github.com/Jiankai-Sun/GC-Net <Br>
https://github.com/kelkelcheng/GC-Net-Tensorflow <Br>
**[Description]** <Br>	
1) 端到端的视差估计方法, 由特征提取, cost volume, 3D卷积三部分组成. 效果较好, 但速度较慢(0.9s) <Br>
	
### **PSMNet ★☆**
**[Paper]** Pyramid Stereo Matching Network<Br>
**[Year]** ECCV 2018 Oral <Br>
**[Author]**  [Jia-Ren Chang](https://jiarenchang.github.io/), [Yong-Sheng Chen](https://people.cs.nctu.edu.tw/~yschen/)<Br>
**[Pages]** <Br>
https://github.com/JiaRenChang/PSMNet <Br>
**[Description]** <Br>	
1) 端到端视差估计网络. 特征提取部分使用了空间金字塔结构, cost volume由左视图和经过相应位移的右视图concat而成, 后续用3D CNN和hourglass结构进行cost volume regularization. <Br>
2) 性能不错, 这一网络结构被后续许多工作采用, 但是速度一般.
	

### **StereoNet ★★**
**[Paper]** StereoNet: Guided Hierarchical Refinement for Real-Time Edge-Aware Depth Prediction<Br>
**[Year]** ECCV 2018 <Br>
**[Author]**  [Sameh Khamis](http://www.samehkhamis.com/), [Sean Fanello](http://www.seanfanello.it/), Christoph Rhemann, Adarsh Kowdle, Julien Valentin, Shahram Izadi<Br>
**[Pages]** <Br>
https://github.com/meteorshowers/StereoNet-ActiveStereoNet <Br>
https://github.com/SPengLiang/StereoNet_Tensorflow <Br>
**[Description]** <Br>	
1) 提出了一个实时的视差估计网络, 分为特征提取, cost volume filtering, refinement三部分, 每部分都使典型的CNN结构. 网络整体结构简单, 速度快(60fps on Titan X), 效果还可以. <Br>
2) 3d Conv还不清楚是怎么用的, 需要之后参考源码.
	
### **iResNet ★★**
**[Paper]** Learning for Disparity Estimation Through Feature Constancy<Br>
**[Year]** CVPR 2018 <Br>
**[Author]**  Zhengfa Liang, Yiliu Feng, [Yulan Guo](http://yulanguo.me/), Hengzhu Liu, Wei Chen, Linbo Qiao, Li Zhou, Jianfeng Zhang<Br>
**[Pages]** <Br>
https://github.com/leonzfa/iResNet <Br>
https://github.com/luoru/iResNet-tf <Br>
**[Description]** <Br>	
1) 粗读，提出一个端到端的视差估计方法, 将特征提取, 视差估计, refine融合进一个网络中. 精度较高, 速度较快(50ms wo refine, 120ms w/ refine). <Br>
2) 没有采用cost volume的策略, 而是采用光流估计中常用的warp+refine策略. <Br>
	
### **MCUA ★**
**[Paper]** Multi-Level Context Ultra-Aggregation for Stereo Matching <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  [Guang-Yu Nie](https://gy-nie.net/), [Ming-Ming Cheng](https://mmcheng.net/cmm/), [Yun Liu](https://mmcheng.net/yliu/), Zhengfa Liang, [Deng-Ping Fan](http://dpfan.net/), Yue Liu, Yongtian Wang<Br>
**[Pages]** <Br>
http://mmcheng.net/mcua/ <Br>
**[Description]** <Br>	
1) 在PSMNet的基础上设计了MCUA结构, 就是类似于densenet的各种密集连接. 虽然参数不多, 但速度较慢(0.9s), 性能较好. <Br>
	
### **GA-Net**
**[Paper]** GA-Net: Guided Aggregation Net for End-To-End Stereo Matching <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  [Feihu Zhang](http://www.feihuzhang.com/), [Victor Prisacariu](http://www.robots.ox.ac.uk/~victor/), [Ruigang Yang](http://research.baidu.com/People/index-view?id=114), [Philip H.S. Torr](http://www.robots.ox.ac.uk/~phst/)<Br>
**[Pages]** <Br>
https://github.com/feihuzhang/GANet <Br>
**[Description]** <Br>	
	
### ***Guided Stereo***
**[Paper]** Guided Stereo Matching <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**   [Matteo Poggi](https://vision.disi.unibo.it/~mpoggi/), Davide Pallotti, [Fabio Tosi](https://vision.disi.unibo.it/~ftosi/), [Stefano Mattoccia](https://vision.disi.unibo.it/~smatt/Site/Home.html)<Br>
**[Pages]** <Br>
https://github.com/mattpoggi/guided-stereo <Br>
**[Description]** <Br>	

### **RF-Net** (非立体匹配)
**[Paper]** RF-Net: An End-To-End Image Matching Network Based on Receptive Field <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**   Xuelun Shen, Cheng Wang, [Xin Li](http://www.ece.lsu.edu/xinli/), Zenglei Yu, [Jonathan Li](https://uwaterloo.ca/mobile-sensing/people-profiles/jonathan-li), Chenglu Wen, Ming Cheng, Zijian He<Br>
**[Pages]** <Br>
**[Description]** <Br>	
	
### **SDC**
**[Paper]** SDC - Stacked Dilated Convolution: A Unified Descriptor Network for Dense Matching Tasks <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**   [Rene Schuster](https://av.dfki.de/members/schuster/), [Oliver Wasenmuller](https://av.dfki.de/members/wasenmueller/), Christian Unger, [Didier Stricker](https://av.dfki.de/members/stricker/)<Br>
**[Pages]** <Br>
**[Description]** <Br>	
	
### **MADNet ★★**
**[Paper]** Real-time self-adaptive deep stereo <Br>
**[Year]** CVPR 2019 Oral <Br>
**[Author]**  Alessio Tonioni, Fabio Tosi, Matteo Poggi, Stefano Mattoccia, Luigi Di Stefano<Br>
**[Pages]** <Br>
https://github.com/CVLAB-Unibo/Real-time-self-adaptive-deep-stereo<Br>
**[Description]** <Br>	
	
### **HSM**
**[Paper]** Hierarchical Deep Stereo Matching on High- Resolution Images<Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  [Gengshan Yang](http://www.contrib.andrew.cmu.edu/~gengshay/wordpress/), [Joshua Manela](http://joshmanela.me/about/), Michael Happold, [Deva Ramanan](https://www.cs.cmu.edu/~deva/)<Br>
**[Pages]** <Br>
http://www.contrib.andrew.cmu.edu/~gengshay/cvpr19stereo<Br>
https://github.com/gengshan-y/high-res-stereo <Br>
**[Description]** <Br>	
	
### **DeepPruner**
**[Paper]** DeepPruner: Learning Efficient Stereo Matching via Differentiable PatchMatch <Br>
**[Year]** ICCV 2019 <Br>
**[Author]**  Shivam Duggal, [Shenlong Wang](http://www.cs.toronto.edu/~slwang/), [Wei-Chiu Ma](http://people.csail.mit.edu/weichium/), Rui Hu, [Raquel Urtasun](http://www.cs.toronto.edu/~urtasun/)<Br>
**[Pages]** <Br>
**[Description]** <Br>	
	
### **RTSNet**
**[Paper]** Real-Time Semantic Stereo Matching <Br>
**[Year]** arXiv 1910 <Br>
**[Author]**  Pier Luigi Dovesi, [Matteo Poggi](https://vision.disi.unibo.it/~mpoggi/), Lorenzo Andraghetti, Miquel Martí, [Hedvig Kjellström](http://www.csc.kth.se/~hedvig/), [Alessandro Pieropan](http://robocoffee.org/), [Stefano Mattoccia](https://vision.disi.unibo.it/~smatt/Site/Home.html)<Br>
**[Pages]** <Br>
**[Description]** <Br>		

## Traditional Matching
### **SGM GPU**
**[Paper]**  Embedded real-time stereo estimation via Semi-Global Matching on the GPU <Br>
**[Year]** ICCS 2016 <Br>
**[Author]**  [D. Hernandez-Juarez](http://danihernandez.eu/), A. Chacón, A. Espinosa, [D. Vázquez](http://www.david-vazquez.com/), J. C. Moure, A. M. López<Br>
**[Pages]** <Br>
https://github.com/dhernandez0/sgm <Br>
**[Description]** <Br>	
	
## Unsupervised Matching
### ***Unsupervised Learning of Stereo Matching***
**[Paper]** Unsupervised Learning of Stereo Matching<Br>
**[Year]** ICCV 2017 <Br>
**[Author]** Chao Zhou, Hong Zhang, [Xiaoyong Shen](http://xiaoyongshen.me/), [Jiaya Jia](http://jiaya.me/)<Br>
**[Pages]** <Br>
**[Description]** <Br>	
	
### **SsSMnet ★★**
**[Paper]** Self-Supervised Learning for Stereo Matching with Self-Improving Ability<Br>
**[Year]** arXiv 1709 <Br>
**[Author]** [Yiran Zhong](https://cecs.anu.edu.au/people/yiran-zhong), [Yuchao Dai](http://users.cecs.anu.edu.au/~yuchao/), Hongdong Li<Br>
**[Pages]** <Br>
**[Description]** <Br>	

### ***Unsupervised Stereo Matching Using Confidential Correspondence Consistency* ★**
**[Paper]** Unsupervised Stereo Matching Using Confidential Correspondence Consistency<Br>
**[Year]** ICIP 2017 <Br>
**[Author]**  Sunghun Joung, [Seungryong Kim](https://seungryong.github.io/), Kihong Park, and Kwanghoon Sohn<Br>
**[Pages]** <Br>
**[Description]** <Br>	
1) 提出了一些计算loss时可靠positive samples挖掘的策略, 包括去除视差过大区域, 选择两张图像颜色相近的区域, 选择梯度大的区域等. <Br>
	
### **ActiveStereoNet ★★**
**[Paper]** ActiveStereoNet:End-to-End Self-Supervised Learning for Active Stereo Systems<Br>
**[Year]** ECCV 2018 Oral<Br>
**[Author]** Yinda Zhang, [Sameh Khamis](http://www.samehkhamis.com/), Christoph Rhemann, Julien Valentin, Adarsh Kowdle, Vladimir Tankovich, Michael Schoenberg, Shahram Izadi, Thomas Funkhouser, [Sean Fanello](http://www.seanfanello.it/)<Br>
**[Pages]** <Br>
https://github.com/meteorshowers/StereoNet-ActiveStereoNet <Br>
**[Description]** <Br>	

### **L2A ★**
**[Paper]** Learning to Adapt for Stereo<Br>
**[Year]** CVPR 2019<Br>
**[Author]** [Alessio Tonioni](https://alessiotonioni.github.io/), Oscar Rahnama, [Thomas Joy](http://www.robots.ox.ac.uk/~tomjoy/), Luigi Di Stefano, [Thalaiyasingam Ajanthan](https://tajanthan.github.io/), [Philip H.S. Torr](http://www.robots.ox.ac.uk/~phst/)<Br>
**[Pages]** <Br>
https://github.com/CVLAB-Unibo/Learning2AdaptForStereo <Br>
**[Description]** <Br>			
  
# Flow And Disparity
## Deep Flow And Disparity
### ***Bridging Stereo Matching and Optical Flow* ★**
**[Paper]** Bridging Stereo Matching and Optical Flow via Spatiotemporal Correspondence <Br>
**[Year]** CVPR 2019 <Br>
**[Author]**  [Hsueh-Ying Lai](https://lelimite4444.github.io/), [Yi-Hsuan Tsai](https://sites.google.com/site/yihsuantsai/), [Wei-Chen Chiu](https://walonchiu.github.io/)<Br>
**[Pages]** <Br>
https://lelimite4444.github.io/BridgeDepthFlow-Project-Page/ <Br>
**[Description]** <Br>	
1)粗读, 提出了一个将匹配和光流估计结合起来的无监督学习框架. 性能还不错. <Br>

## Traditional Flow And Disparity
### ***Fast Cost-Volume Filtering***
**[Paper]** Fast Cost-Volume Filtering for Visual Correspondence and Beyond <Br>
**[Year]** PAMI 2013 <Br>
**[Author]** Asmaa Hosni, Christoph Rhemann, Michael Bleyer, Carsten Rother, Margrit Gelautz<Br>
**[Pages]** <Br>
https://github.com/fjordyo0707/StereoMatching-CostFilter <Br>
**[Description]** <Br>	
	
# Datasets
[Sintel](http://sintel.is.tue.mpg.de/)  Stereo Matching + Optical FLow

[KITTI](http://www.cvlibs.net/datasets/kitti/)  Stereo Matching + Optical FLow

[UCF 101](https://www.crcv.ucf.edu/data/UCF101.php)

[Middlebury](http://vision.middlebury.edu/)  Stereo Matching + Optical FLow <Br>
Paper: A taxonomy and evaluation of dense two-frame stereo correspondence algorithms

[Scene Flow](https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html)  Stereo Matching + Optical FLow<Br>
Paper: A Large Dataset to Train Convolutional Networks for Disparity, Optical Flow, and Scene Flow Estimation

[DrivingStereo](https://drivingstereo-dataset.github.io/) Stereo Matching <Br>
Paper: DrivingStereo: A Large-Scale Dataset for Stereo Matching in Autonomous Driving Scenarios


# Leaderboards
[KITTI Flow 2012 Leaderboard](http://www.cvlibs.net/datasets/kitti/eval_stereo_flow.php?benchmark=flow)

[KITTI Flow 2015 Leaderboard](http://www.cvlibs.net/datasets/kitti/eval_scene_flow.php?benchmark=flow)

[KITTI Stereo 2012 Leaderboard](http://www.cvlibs.net/datasets/kitti/eval_stereo_flow.php?benchmark=stereo)

[KITTI Stereo 2015 Leaderboard](http://www.cvlibs.net/datasets/kitti/eval_scene_flow.php?benchmark=stereo)

# Projects
http://ccwu.me/vsfm/
