---
layout: home2
permalink: /projects/
title: Research interest
tags: [tools]
modified: 6-3-2018
comments: false


---
<br>
### Connected vehicles
----

<div class="post-container"> 
    <div class="post-content">
        <h3 class="post-title">The see-through system</h3>
        <p>In this collaboration with Bosch, we propose a real-time marker-less system to see through cars. For this purpose, two cars are equipped with cameras and an appropriate wireless communication system. The stereo vision system mounted on the front car allows to create a sparse 3D map of the environment where the rear car can be localized. Using this inter-car pose estimation, a synthetic image is generated to overcome the occlusion and to create a seamless see-through effect which preserves the structure of the scene. 
 <a href="http://www.youtube.com/watch?feature=player_embedded&v=RYzgyOgVzM4">[Video]</a> 
<a href="https://www.researchgate.net/publication/305695638_A_Real-time_Augmented_Reality_System_to_See-Through_Cars">[TVCG16, </a>
<a href="https://link.springer.com/chapter/10.1007/978-3-319-48881-3_15">ECCVW16]</a>

 </p></div>
<div class="post-thumb"><img src="/images/STC-2.png" /></div>
</div>
<br />

<div class="post-container">
    <div class="post-content">
        <h3 class="post-title">Collaborative localization of a swarm of vehicle</h3>
        <p>We also proposed an extension of the two car see-through system for an arbitrary number of vehicle. Specifically, we created a multi-vehicle localization approach relying exclusively on cameras installed on connected cars (i.e. vehicles with Internet access). The proposed method is designed to perform in real-time while requiring a low bandwidth connection as a result of an efficient centralized/decentralized architecture. Hence, our approach is compatible with both LTE Internet connection and local WIFI networks. To reach this goal, the vehicles share small portions of their respective 3D maps to estimate their relative positions. The global consistency between multiple vehicles is enforced via a novel graph-based strategy. This work is still under review for a journal publication.
<a href="https://www.youtube.com/watch?v=GD7Z95bWP6k&t=38s">[Video]</a> 
</p></div>
<div class="post-thumb"><img src="/images/IllustMultiCar.png" /></div>
</div>


<div class="post-container">
    <div class="post-content">
        <h3 class="post-title"> Smart city</h3>
        <p> I develloped novel solutions for semi-automatic CCTV camera calibration and 3D vehicle detection/tracking/geo-localization in the context of smart city.The paper is currently under review but you are welcome to check the calibration toolbox I develloped <a href="https://github.com/rameau-fr/CCTV-Calib">[CCTV-Calib]</a> and the video results obtained for 3D vehicle localization from our domain adaption strategy <a href="https://www.youtube.com/watch?v=KcbXZZcCmag">[Video-1]</a> <a href="https://www.youtube.com/watch?v=24Iw_wvUmjE&t=193s">[Video-2]</a>
</p></div>
<div class="post-thumb"><img src="/images/3D_vehicles.png" /></div>
</div>


---
<br>
### Camera calibration
----


<div class="post-container">
    <div class="post-content">
<h3 class="post-title">Multi-camera calibration</h3>
        <p> In this paper, we present MC-Calib, a novel and robust toolbox dedicated to the calibration of complex synchronized multi-camera systems using an arbitrary number of fiducial marker-based patterns. Calibration results are obtained via successive stages of refinement to reliably estimate both the poses of the calibration boards and cameras in the system. Our method is not constrained by the number of cameras, their overlapping field-of-view (FoV), or the number of calibration patterns used. Moreover, neither prior information about the camera system nor the positions of the checkerboards are required. As a result, minimal user interaction is needed to achieve an accurate and robust calibration which makes this toolbox accessible even with limited computer vision expertise. In this work, we put a strong emphasis on the versatility and the robustness of our technique. Specifically, the hierarchical nature of our strategy allows to reliably calibrate complex vision systems even under the presence of noisy measurements. Additionally, we propose a new strategy for best-suited image selection and initial parameters estimation dedicated to non-overlapping FoV cameras. Finally, our calibration toolbox is compatible with both, perspective and fisheye cameras. Our solution has been validated on a large number of real and synthetic sequences including monocular, stereo, multiple overlapping cameras, non-overlapping cameras, and converging camera systems. <a href="https://github.com/rameau-fr/MC-Calib">[Project]</a>.
</p></div>
<div class="post-thumb"><img src="/images/illustration-MCCalib.png" /></div>
</div>

<div class="post-container">
    <div class="post-content">
<h3 class="post-title">PTZ self-calibration</h3>
        <p> Rotating and zooming cameras, also called PTZ (Pan-Tilt-Zoom) cameras, are widely used in modern surveil-lance systems. While their zooming ability allows acquiring detailed images of the scene, it also makes their cali-bration more challenging since any zooming action results in a modification of their intrinsic parameters. I designed multiple techniques for the particular case of Pan-Tilt-Zoom camera calibration. One of my fist paper  <a href="https://www.researchgate.net/publication/232614240_Self-calibration_of_a_PTZ_Camera_Using_New_LMI_Constraints">[ACCV12]</a>  focuses on the construction of new LMI constraints to robustly obtain compute the intrinsic parameters of a camera from a set of images.
More recently, we proposed an extension of such work using CNN to regress the calibration parameters of a rotating and zooming camera (join estimation of rotation, radial distortion and projection parameters) <a href="http://openaccess.thecvf.com/content_WACV_2020/html/Zhang_DeepPTZ_Deep_Self-Calibration_for_PTZ_Cameras_WACV_2020_paper.html">[WACV20]</a>.
</p></div>
</div>

<br />

<div class="post-container">
    <div class="post-content">
<h3 class="post-title">Deep-learning based camera calibration</h3>
        <p>Calibration of wide field-of-view cameras is a fundamental step for numerous visual media production applications, such as 3D reconstruction, image undistortion, augmented reality and camera motion estimation. However, existing calibration methods require multiple images of a calibration pattern (typically a checkerboard), assume the presence of lines, require manual interaction and/or need an image sequence. In contrast, we present a novel fully automatic deep learning-based approach that overcomes all these limitations and works with a single image of general scenes. Our approach builds upon the recent developments in deep Convolutional Neural Networks (CNN): our network automatically estimates the intrinsic parameters of the camera (focal length and distortion parameter) from a single input image. For more details, please have on look on our project webpage 
<a href="https://github.com/alexvbogdan/DeepCalib">[WebPage]</a>
<a href="https://drive.google.com/file/d/1pZgR3wNS6Mvb87W0ixOHmEVV6tcI8d50/view">[CVMP19]</a>.
<div class="post-thumb"><img src="/images/Undistord.png"/></div>
</p></div>
</div>

<div class="post-container">
    <div class="post-content">
<h3 class="post-title">Head-eye calibration</h3>
        <p>Through my research career, I encounter multiple scenarios involving hand-eye calibration problems. In particular in case of non-overlapping field-of-view cameras and when the camera is attached to a static referencial. For more details you can have a look into the related papers 
<a href="https://tel.archives-ouvertes.fr/tel-01128289/file/2014DIJOS031.pdf">[PhD14, </a>
<a href="https://link.springer.com/chapter/10.1007/978-3-319-48881-3_15">ECCVW16]</a>.
</p></div>
</div>



---
<br>
### Detection and Visual tracking
----



<div class="post-container">
    <div class="post-content">
<h3 class="post-title">Deep-learning based tracking</h3>
        <p>We propose a novel video object segmentation algorithm based on pixel-level matching using Convolutional Neural Networks (CNN). Our network aims to distinguish the target area from the background on the basis of the pixel-level similarity between two object units. The proposed network represents a target object using features from different depth layers in order to take advantage of both the spatial details and the category-level semantic information. Furthermore, we propose a feature compression technique that drastically reduces the memory requirements while maintaining the capability of feature representation. Two-stage training (pre-training and fine-tuning) allows our network to handle any target object regardless of its category (even if the object’s type does not belong to the pre-training data) or of variations in its appearance through a video sequence. Experiments on large datasets demonstrate the effectiveness of our model - against related methods - in terms of accuracy, speed, and stability. Finally, we introduce the transferability of our network to different domains, such as the infrared data domain. 

<a href="https://jsyoon4325.wixsite.com/pix-matching">[WebPage]</a>
<div class="post-thumb"><img src="/images/DeepTrack.png" /></div> 
</p></div>
</div>


<div class="post-container">
<h3 class="post-title">Omidirectional camera visual tracking</h3>
    <div class="post-content">
        <p>One of the first research work I accomplished was the devellopment of novel visual tracking techniques for omnidirectional cameras. More details here:  
 <a href="http://www.youtube.com/watch?feature=player_embedded&v=GL33I-zMLB4">[Video]</a> 
<a href="https://hal-univ-bourgogne.archives-ouvertes.fr/file/index/docid/627905/filename/2011_rameau_omnivis.pdf">[ICCVW11, </a>
<a href="http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.658.1888&rep=rep1&type=pdf">EL11]</a>
</p></div>
</div>

<div class="post-container">
    <div class="post-content">
<h3 class="post-title">3D car detection</h3>
        <p>Recent 3D object localization approaches have speed bottleneck caused by the fusion/prediction of depth information or anchor generation. To alleviate this issue, in this paper, we present a monocular 3D car localization method that takes advantage of road environments, i.e., car on the ground surface, instead of full depth estimation. Concretely, we propose two stages approach consists of segment and regression networks, called Segment2Regress. Given a single RGB image and a prior 2D object detection bounding box, 1) the segment network activates the pixels under the vehicles, which correspond to four line segments and a quadrilateral of the bottom of a vehicle 3D box projected on the image domain, and then, 2) the regression network predicts the 3D location of a car at the ground level. We stabilize the regression by introducing the coupling loss for grouping regression. Thanks to its simple structure, the proposed method is light and efficient and reach up to 80 FPS. 
<a href="http://rss2019.informatik.uni-freiburg.de/papers/0079_FI.pdf">[RSS19]</a>
<div class="post-thumb"><img src="/images/Seg2Reg.png" /></div> 
</p></div>
</div>


---
<br>
### 3D reconstruction
----


<div class="post-container">
    <div class="post-content">
        <h3 class="post-title">stereo-SLAM</h3>
        <p> I fully devellop my own stereo-SLAM. You can have a look here for a small demo on KITTI  
<a href="http://www.youtube.com/watch?feature=player_embedded&v=5g5Uu7XX_Hk">[Video]</a>.
You can also have a look at our paper on keypoints detection <a href="https://github.com/BAILOOL/ANMS-Codes">[PRL18]</a>.
 </p></div>
</div>


<div class="post-container">
    <div class="post-content">
<h3 class="post-title">360° reconstruction</h3>
<p> 
With the growing use of head-mounted displays for virtualreality (VR), generating 3D contents for these devices becomes an impor-tant topic in computer vision. For capturing full 360 degree panoramasin a single shot, the Spherical Panoramic Camera (SPC) are gaining inpopularity. However, estimating depth from a SPC remains a challeng-ing problem. In this paper, we propose a practical method that generatesall-around dense depth map using a narrow-baseline video clip capturedby a SPC. While existing methods for depth from small motion rely onperspective cameras, we introduce a new bundle adjustment approachtailored for SPC that minimizes the re-projection error directly on theunit sphere. It enables to estimate approximate metric camera posesand 3D points. Additionally, we present a novel dense matching methodcalled sphere sweeping algorithm. This allows us to take advantage of theoverlapping regions between the cameras <a href="https://sunghoonim.github.io/assets/paper/ECCV16_Allaround.pdf">[ECCV16]</a>.
<div class="post-thumb"><img src="/images/360Recon.png" /></div> 
</p></div>
</div>


---
<br>
### Others: Domain adaptation, NERF, 3D point cloud processing and much more
----



