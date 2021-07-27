
# Stereo Matching
- [Deep Matching](#deep-matching)
- [Traditional Matching](#traditional-matching)


## Deep Matching
### **RTSNet**
**[Paper]** Real-Time Semantic Stereo Matching <Br>
**[Year]** arXiv 1910 <Br>
**[Author]**  Pier Luigi Dovesi, [Matteo Poggi](https://vision.disi.unibo.it/~mpoggi/), Lorenzo Andraghetti, Miquel Martí, [Hedvig Kjellström](http://www.csc.kth.se/~hedvig/), [Alessandro Pieropan](http://robocoffee.org/), [Stefano Mattoccia](https://vision.disi.unibo.it/~smatt/Site/Home.html)<Br>
**[Pages]** <Br>
**[Description]** <Br>	
  
### **DeepPruner**
**[Paper]** DeepPruner: Learning Efficient Stereo Matching via Differentiable PatchMatch <Br>
**[Year]** ICCV 2019 <Br>
**[Author]**  Shivam Duggal, [Shenlong Wang](http://www.cs.toronto.edu/~slwang/), [Wei-Chiu Ma](http://people.csail.mit.edu/weichium/), Rui Hu, [Raquel Urtasun](http://www.cs.toronto.edu/~urtasun/)<Br>
**[Pages]** <Br>
**[Description]** <Br>	
	
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
	

	

	

  
  
  
## Traditional Matching

### **L2A ★**
**[Paper]** Learning to Adapt for Stereo<Br>
**[Year]** CVPR 2019<Br>
**[Author]** [Alessio Tonioni](https://alessiotonioni.github.io/), Oscar Rahnama, [Thomas Joy](http://www.robots.ox.ac.uk/~tomjoy/), Luigi Di Stefano, [Thalaiyasingam Ajanthan](https://tajanthan.github.io/), [Philip H.S. Torr](http://www.robots.ox.ac.uk/~phst/)<Br>
**[Pages]** <Br>
https://github.com/CVLAB-Unibo/Learning2AdaptForStereo <Br>
**[Description]** <Br>			
	
### **ActiveStereoNet ★★**
**[Paper]** ActiveStereoNet:End-to-End Self-Supervised Learning for Active Stereo Systems<Br>
**[Year]** ECCV 2018 Oral<Br>
**[Author]** Yinda Zhang, [Sameh Khamis](http://www.samehkhamis.com/), Christoph Rhemann, Julien Valentin, Adarsh Kowdle, Vladimir Tankovich, Michael Schoenberg, Shahram Izadi, Thomas Funkhouser, [Sean Fanello](http://www.seanfanello.it/)<Br>
**[Pages]** <Br>
https://github.com/meteorshowers/StereoNet-ActiveStereoNet <Br>
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
	

## Unsupervised Matching
### ***Unsupervised Learning of Stereo Matching***
**[Paper]** Unsupervised Learning of Stereo Matching<Br>
**[Year]** ICCV 2017 <Br>
**[Author]** Chao Zhou, Hong Zhang, [Xiaoyong Shen](http://xiaoyongshen.me/), [Jiaya Jia](http://jiaya.me/)<Br>
**[Pages]** <Br>
**[Description]** <Br>	
  
 ### **SGM GPU**
**[Paper]**  Embedded real-time stereo estimation via Semi-Global Matching on the GPU <Br>
**[Year]** ICCS 2016 <Br>
**[Author]**  [D. Hernandez-Juarez](http://danihernandez.eu/), A. Chacón, A. Espinosa, [D. Vázquez](http://www.david-vazquez.com/), J. C. Moure, A. M. López<Br>
**[Pages]** <Br>
https://github.com/dhernandez0/sgm <Br>
**[Description]** <Br>	 
  
### DASC ★
**[Paper]** DASC: Dense Adaptive Self-Correlation Descriptor for Multi-modal and Multi-spectral Correspondence <Br>
**[Year]** CVPR 2015 <Br>
**[Author]** [Seungryong Kim](https://seungryong.github.io/), [Dongbo Min](http://cvl.ewha.ac.kr/), [Bumsub Ham](https://bsham.github.io/), Seungchul Ryu, Minh N. Do, Kwanghoon Sohn<Br>
**[Pages]** <Br>
https://seungryong.github.io/DASC/ <Br>
**[Description]** <Br>	
