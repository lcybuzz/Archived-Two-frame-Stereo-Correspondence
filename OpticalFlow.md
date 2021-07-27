# Optical Flow Estimation
  - [Deep Optical Flow](#deep-optical-flow)
  - [Traditional Optical Flow](#traditional-optical-flow)
  - [Unsupervised Optical Flow](#unsupervised-optical-flow)


## Deep Optical Flow
### MaskFlownet ★☆
**[Paper]** (CVPR 020 Oral) MaskFlownet: Asymmetric Feature Matching with Learnable Occlusion Mask <Br>
**[Author]** Shengyu Zhao, Yilun Sheng, Yue Dong, [Eric I-Chao Chang](https://www.microsoft.com/en-us/research/people/echang/?from=http%3A%2F%2Fresearch.microsoft.com%2Fen-us%2Fpeople%2Fechang%2F), Yan Xu <Br>
**[[MXNet-Code](https://github.com/microsoft/MaskFlownet)]**<Br>
隐式预测occlusion map
	
### IRR ★
**[Paper]** (CVPR 2019) Iterative Residual Refinement for Joint Optical Flow and Occlusion Estimation <Br>
**[Author]** [Junhwa Hur](https://hurjunhwa.github.io/), [Stefan Roth](https://www.visinf.tu-darmstadt.de/visinf/team_members/sroth/sroth.en.jsp) <Br>
**[[Pytorch-Code](https://github.com/visinf/irr)]**<Br>

### Bridging Stereo Matching and Optical Flow ★
**[Paper]** (CVPR 2019) Bridging Stereo Matching and Optical Flow via Spatiotemporal Correspondence <Br>
**[Author]**  [Hsueh-Ying Lai](https://lelimite4444.github.io/), [Yi-Hsuan Tsai](https://sites.google.com/site/yihsuantsai/), [Wei-Chen Chiu](https://walonchiu.github.io/)<Br>
**[[Project](https://lelimite4444.github.io/BridgeDepthFlow-Project-Page/)]** <Br>
1)粗读, 提出了一个将匹配和光流估计结合起来的无监督学习框架. 性能还不错. <Br>

### PWC-Net ★★
**[Paper]** (CVPR 2018 Oral) PWC-Net: CNNs for Optical Flow Using Pyramid, Warping, and Cost Volum <Br>
**[Author]** Deqing Sun, [Xiaodong Yang](http://xiaodongyang.org/), [Ming-Yu Liu](http://mingyuliu.net/), [Jan Kautz](http://jankautz.com/) <Br>
**[[Project](https://research.nvidia.com/publication/2018-02_PWC-Net:-CNNs-for)]** **[[Code](https://github.com/NVlabs/PWC-Net)]** **[[Code](https://github.com/philferriere/tfoptflow)]**<Br>

### LiteFlowNet ★☆
**[Paper]** (CVPR 2018 Spotlight) LiteFlowNet: A Lightweight Convolutional Neural Network for Optical Flow Estimation <Br>
**[Author]** Tak-Wai Hui, [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[[Project](http://mmlab.ie.cuhk.edu.hk/projects/LiteFlowNet/)]** **[[Code](https://github.com/twhui/LiteFlowNet)]**<Br>
1) 粗读。轻量级光流估计网络，效果和速度都不错. <Br>
2) 采用encoder-decoder结构，逐级估计光流+warp，每个level估计光流时设计了matching+refine两阶段结构. <Br>
3) 另外提出了一个flow regularization策略，对预测的光流进行滤波，其中滤波的kernel是通过网络学习出来的. 感觉作用类似于一个边缘保持滤波器. <Br>

### LiteFlowNet2
**[Paper]** (TPAMI 2019) A Lightweight Optical Flow CNN - Revisiting Data Fidelity and Regularization <Br>
**[Author]** Tak-Wai Hui, [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[[Code](https://github.com/twhui/LiteFlowNet2)]** <Br>
	
### SpyNet
**[Paper]** (CVPR 2017) SPyNet: Spatial Pyramid Network for Optical Flow <Br>
**[Author]** Anurag Ranjan, [Michael J. Black](https://ps.is.tuebingen.mpg.de/person/black) <Br>
**[[Code](https://github.com/anuragranj/spynet)]**<Br>

### FlowNet ★★☆
**[Paper]** (ICCV 2015) FlowNet: Learning Optical Flow with Convolutional Networks <Br>
**[Author]** Alexey Dosovitskiy, Philipp Fischer, Eddy Ilg, P. Häusser, C. Hazırbaş, V. Golkov, P. Smagt, D. Cremers, Thomas Brox <Br>
**[[Project](https://lmb.informatik.uni-freiburg.de/Publications/2015/DFIB15/)]** <Br>

	
### FlowNet 2.0 ★
**[Paper]** (CVPR 2017) FlowNet 2.0: Evolution of Optical Flow Estimation with Deep Networks <Br>
**[Author]** Eddy Ilg, Nikolaus Mayer, Tonmoy Saikia, Margret Keuper, Alexey Dosovitskiy, Thomas Brox <Br>
**[[Project](https://lmb.informatik.uni-freiburg.de/resources/software.php)]**  **[[Code](https://github.com/lmb-freiburg/flownet2)]** **[[Pytorch-Code](https://github.com/NVIDIA/flownet2-pytorch)]** <Br>
1) FlowNet的改进版, 用了stack等策略. 效果还可以, 但不知在真实数据上的性能有没有保证. <Br>
2) 整篇论文就像一个实验报告, 细节还没研究. <Br>	









## Traditional Optical Flow

### **BriefMatch**
**[Paper]** (SCIA17) BriefMatch: Dense binary feature matching for real-time optical flow estimation  <Br>
**[Year]**  <Br>
**[Author]** [Gabriel Eilertsen](http://vcl.itn.liu.se/members/gabriel-eilertsen), Per-Erik Forssén, [Jonas Unger](http://vcl.itn.liu.se/members/jonas-unger) <Br>
**[[Code](https://github.com/gabrieleilertsen/briefmatch)]**  <Br>	
	
### ***Optical Flow Filter***
**[Paper]** (RAL 2016) A Filter Formulation for Computing Real Time Optical Flow <Br>
**[Author]** [Juan David Adarve](http://jadarve.github.io/), David J. Austin, [Robert Mahony](https://users.cecs.anu.edu.au/~Robert.Mahony/) <Br>
**[[Code](https://github.com/jadarve/optical-flow-filter)]**  <Br>

### **DIS**
**[Paper]** (CVPR 2016) Fast Optical Flow using Dense Inverse Search  <Br>
**[Author]** Till Kroeger, [Radu Timofte](http://www.vision.ee.ethz.ch/~timofter/), [Dengxin Dai](http://www.vision.ee.ethz.ch/~daid/), Luc Van Gool <Br>
**[[Code](https://github.com/tikroeger/OF_DIS)]**  <Br>

### Fast Cost-Volume Filtering
**[Paper]** (TPAMI 2013) Fast Cost-Volume Filtering for Visual Correspondence and Beyond <Br>
**[Author]** Asmaa Hosni, Christoph Rhemann, Michael Bleyer, Carsten Rother, Margrit Gelautz<Br>
**[[Code](https://github.com/fjordyo0707/StereoMatching-CostFilter)]**  <Br>	
	
	
	
	
## Unsupervised Optical Flow
### SelFlow ★
**[Paper]** (CVPR 2019 Oral) SelFlow: Self-Supervised Learning of Optical Flow <Br>
**[Author]**   [Pengpeng liu](https://ppliuboy.github.io/), [Michael R. Lyu](http://www.cse.cuhk.edu.hk/lyu/), [Irwin King](https://www.cse.cuhk.edu.hk/irwin.king/), [Jia Xu](http://pages.cs.wisc.edu/~jiaxu/index.html)<Br>
**[[Code](https://github.com/ppliuboy/SelFlow )]**  <Br>

### CC ★★
**[Paper]** (CVPR 2019) Competitive Collaboration: Joint Unsupervised Learning of Depth, Camera Motion, Optical Flow and Motion Segmentation <Br>
**[Author]**  Anurag Ranjan, Varun Jampani,Lukas Balles, [Kihwan Kim](https://www.cc.gatech.edu/~kihwan23/), Deqing Sun, Jonas Wulff , [Michael J. Black](https://ps.is.tuebingen.mpg.de/person/black)<Br>
**[[Project](https://research.nvidia.com/publication/2018-05_Adversarial-Collaboration-Joint)]** **[[Code](https://github.com/anuragranj/cc)]**   <Br>	
1) 大致浏览, 提出一种非监督的联合估计深度, 相机姿态, 光流以及运动物体分割的框架. 用类似于EM的交替迭代优化策略, 利用任务间的相互制约关系提升每个子任务的性能. <Br>
2) 相机姿态和深度的估计适用于静态区域, 光流估计适用于动态区域, 它们之间是竞争关系, motion segmentation用来充当仲裁者的角色. <Br>
3) 从思路和结果来看感觉这篇文章很有趣, 不过不太适用于当前需求, 以后有需要可以深入了解下. <Br>

### *Unsupervised Event-based Learning of Optical Flow, Depth, and Egomotion*
**[Paper]** (CVPR 2019) Unsupervised Event-based Learning of Optical Flow, Depth, and Egomotion<Br>
**[Author]**  [Alex Zihao Zhu](https://fling.seas.upenn.edu), Liangzhe Yuan, Kenneth Chaney, [Kostas Daniilidis](https://www.cis.upenn.edu/~kostas/)
<Br>

### Robustness Meets Deep Learning
**[Paper]** (arXiv 1812) Robustness Meets Deep Learning: An End-to-End Hybrid Pipeline for Unsupervised Learning of Egomotion <Br>
**[Author]**  [Alex Zihao Zhu](https://fling.seas.upenn.edu), Wenxin Liu, Ziyun Wang, Vijay Kumar, [Kostas Daniilidis](https://www.cis.upenn.edu/~kostas/)
<Br>
	
### **UnFlow ★**
**[Paper]** (AAAI 2018) UnFlow: Unsupervised Learning of Optical Flow with a Bidirectional Census Loss <Br>
**[Author]** Simon Meister, Junhwa Hur,  Stefan Roth <Br>
**[[Code](https://github.com/simonmeister/UnFlow)]**   <Br>

### ***Learning Features by Watching Objects Move***
**[Paper]** (CVPR 2017) Learning Features by Watching Objects Move <Br>
**[Author]** [Deepak Pathak](https://people.eecs.berkeley.edu/~pathak/), [Ross Girshick](http://www.rossgirshick.info/), [Piotr Dollár](https://pdollar.github.io/), [Trevor Darrell](https://people.eecs.berkeley.edu/~trevor/), [Bharath Hariharan](http://home.bharathh.info/) <Br>
**[[Project](https://people.eecs.berkeley.edu/~pathak/unsupervised_video/)]**  <Br>
	
### Unsupervised Flownet ★
**[Paper]** (ECCVW 2016) Back to basics: Unsupervised learning of optical flow via brightness constancy and motion smoothness <Br>
**[Author]** [Jason J. Yu](https://www.eecs.yorku.ca/~jjyu/), [Adam W. Harley](http://www.cs.cmu.edu/~aharley/), [Konstantinos G. Derpanis](http://www.scs.ryerson.ca/~kosta/) <Br>
**[[Project](https://www.eecs.yorku.ca/~jjyu/projects/unsupflow/)]**  **[[TF-Code](https://github.com/ryersonvisionlab/unsupFlownet/)]**    <Br>

### Unsupervised convolutional neural networks for motion estimation
**[Paper]** (ICIP 2016) Unsupervised convolutional neural networks for motion estimation <Br>
**[Author]** Aria Ahmadi, Ioannis Patras <Br>
	


