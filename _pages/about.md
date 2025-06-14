---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. candidate in Electrical and Computer Engineering at the [University of Maryland, College Park](https://ece.umd.edu/), working with [Prof. Shuvra S. Bhattacharyya](https://user.eng.umd.edu/~ssb/) in the [Maryland DSPCAD Research Group](https://code.umd.edu/dspcad-pub/dspcadwiki/-/wikis/Maryland-DSPCAD-Research-Group). I received my M.S. degree from the [Graduate Institute of Electronics Engineering](https://giee.ntu.edu.tw/en/home/) at National Taiwan University, where I was advised by [Prof. Liang-Gee Chen](https://www.ee.ntu.edu.tw/profile1.php?id=26) in the [DSPIC Lab](https://homepage.ntu.edu.tw/~lgchen/index.html). I earned my B.S. degree in Electrical Engineering from [National Taiwan University](https://web.ee.ntu.edu.tw/eng/index.php).

Research
======
My research centers on <em>data-efficient</em> machine learning, with the overarching goal of minimizing human effort required in data annotation and expanding the accessibility of machine learning across a wide range of domains. I am particularly focused on challenging settings, such as <span style="background-color: #ffa69e;">aerial-view</span>, <span style="background-color:rgb(247, 229, 173);">human-centric</span>, <span style="background-color: #b8f2e6;">medical</span>, <span style="background-color: #aed9e0;">robotic</span> perception, where labeled data is scarce or expensive to obtain, and computational resources may be limited.

To support this vision, I have explored a diverse set of machine learning paradigms, including sim-to-real adaptation, generative modeling, multimodal large language models, and self-supervised learning. My work is driven by both theoretical curiosity and practical relevance, targeting real-world constraints in complex environments.

Below is a summary of my research contributions, categorized by methodology and color-coded by application domain:
<div style="font-size: 0.9em; margin-top: 0; margin-bottom: 20px;">
<strong>&bull; Sim-to-Real Adaptation:</strong> <span style="background-color: #ffa69e;"><a href="#synplay" style="color: inherit;">SynPlay [Preprint]</a></span>, <span style="background-color: #ffa69e;"><a href="#ptl" style="color: inherit;">PTL [CVPR'23, <strong>Highlight</strong>]</a></span>, <span style="background-color: #ffa69e;"><a href="#archangel" style="color: inherit;">Archangel [IEEE Access'23]</a></span><br>
<strong>&bull; Generative Modeling:</strong> <span style="background-color: #ffa69e;"><a href="#synposediv" style="color: inherit;">SynPoseDiv [ICIP'25]</a></span><br>
<strong>&bull; Multimodal LLMs:</strong> <span style="background-color:rgb(247, 229, 173);"><a href="#autocompose" style="color: inherit;">AutoComPose [Preprint]</a></span><br>
<strong>&bull; Semi-Supervised, Weakly, and Self-Supervised Learning:</strong> <span style="background-color: #b8f2e6;"><a href="#memo" style="color: inherit;">MEMO [BOE'24]</a></span>, <span style="background-color: #aed9e0;"><a href="#depthweak" style="color: inherit;">What Synthesis is Missing [ICCV'19]</a></span>, <span style="background-color: #aed9e0;"><a href="#depthte" style="color: inherit;">D+T-Net [MS Thesis]</a></span><br>
<strong>&bull; Miscellaneous:</strong> <span style="background-color:rgb(247, 229, 173);"><a href="#egofall" style="color: inherit;">EgoFall [ICASSP'24, TNSRE'25]</a></span>, <span style="background-color: #ffa69e;"><a href="#ddhc" style="color: inherit;">DDHC [WHISPERS'21]</a></span><br>
</div>

Preprints
======
<div style="display: flex; align-items: flex-start; margin-top: 20px; margin-bottom: 20px; position: relative;" id="autocompose">
  <img src="/images/autocompose.jpg" alt="AutoComPose" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      AutoComPose: Automatic Generation of Pose Transition Descriptions for Composed Pose Retrieval Using Multimodal LLMs
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      <strong>Yi-Ting Shen*</strong>, Sungmin Eum*, Doheon Lee, Rohit Shete, Chiao-Yi Wang, Heesung Kwon, and Shuvra S. Bhattacharyya (* equal contribution)
      <br>
      <a href="https://arxiv.org/abs/2503.22884">[arXiv]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We introduce <em>AutoComPose</em>, the first framework to automatically generate pose transition annotations using multimodal large language models, significantly improving composed pose retrieval performance while reducing reliance on costly human labeling.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/autocompose.jpg" alt="AutoComPose Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="synplay">
  <img src="/images/synplay.png" alt="SynPlay" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      SynPlay: Importing Real-world Diversity for a Synthetic Human Dataset
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      Jinsub Yim, Hyungtae Lee, Sungmin Eum, <strong>Yi-Ting Shen</strong>, Yan Zhang, Heesung Kwon, and Shuvra S. Bhattacharyya
      <br>
      <a href="https://arxiv.org/abs/2408.11814">[arXiv]</a> <a href="https://synplaydataset.github.io/">[Project]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We present <em>Synthetic Playground (SynPlay)</em>, a large-scale synthetic human dataset with diverse motions and camera viewpoints—especially aerial views—that significantly improves human identification performance in challenging, data-scarce scenarios like few-shot learning and cross-domain adaptation.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/synplay.png" alt="SynPlay Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="synanalysis">
  <img src="/images/synanalysis.jpg" alt="SynAnalysis" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      Exploring the Impact of Synthetic Data for Aerial-view Human Detection
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      Hyungtae Lee, Yan Zhang, <strong>Yi-Ting Shen</strong>, Heesung Kwon, and Shuvra S. Bhattacharyya
      <br>
      <a href="https://arxiv.org/abs/2405.15203">[arXiv]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We investigate key factors influencing sim-to-real transfer in UAV-based human recognition and reveal how strategic selection of synthetic data can significantly improve model performance and domain generalization, offering insights that challenge common misconceptions about synthetic data usage.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/synanalysis.jpg" alt="SynAnalysis Enlarged" class="enlarged-image">
  </div>
</div>

Publications
======
<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="synposediv">
  <img src="/images/synposediv.jpg" alt="SynPoseDiv" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      Diversifying Human Pose in Synthetic Data for Aerial-view Human Detection
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      <strong>Yi-Ting Shen*</strong>, Hyungtae Lee*, Heesung Kwon, and Shuvra S. Bhattacharyya (* equal contribution)
      <br>
      <em>ICIP 2025</em>
      <br>
      <a href="https://arxiv.org/abs/2405.15939">[arXiv]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We introduce <em>SynPoseDiv</em>, a novel framework that enhances synthetic aerial-view datasets by generating realistic and diverse 3D human poses using diffusion models and image translation, leading to significantly improved detection accuracy, especially in low-shot scenarios.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/synposediv.jpg" alt="SynPoseDiv Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-top: 20px; margin-bottom: 20px; position: relative;" id="egofall">
  <img src="/images/egofall.jpg" alt="EgoFall" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      EgoFall: Real-time Privacy-Preserving Fall Risk Assessment with a Single On-Body Tracking Camera
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      Chiao-Yi Wang, Faranguisse Kakhi Sadrieh, <strong>Yi-Ting Shen</strong>, Giovanni Oppizzi, Li-Qun Zhang, and Yang Tao
      <br>
      <em>ICASSP 2024</em>
      <br>
      <em>IEEE Transactions on Neural Systems and Rehabilitation Engineering 2025</em>
      <br>
      <a href="https://ieeexplore.ieee.org/document/10447770">[Conference Paper]</a> <a href="https://ieeexplore.ieee.org/abstract/document/11027155">[Journal Extension]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We propose <em>EgoFall</em>, a real-time, privacy-preserving fall risk assessment system that uses a chest-mounted camera and a lightweight CNN-Transformer model to analyze ego-body motion, enabling personalized fall prevention without relying on multiple wearable sensors.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/egofall.jpg" alt="EgoFall Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="memo">
  <img src="/images/memo.jpg" alt="MEMO" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      MEMO: Dataset and Methods for Robust Multimodal Retinal Image Registration with Large or Small Vessel Density Differences
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      Chiao-Yi Wang, Faranguisse Kakhi Sadrieh, <strong>Yi-Ting Shen</strong>, Shih-En Chen, Sarah Kim, Victoria Chen, Achyut Raghavendra, Dongyi Wang, Osamah Saeedi, and Yang Tao
      <br>
      <em>Biomedical Optics Express 2024</em>
      <br>
      <a href="https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-3457&id=549452">[Paper]</a> <a href="https://chiaoyiwang0424.github.io/MEMO/">[Dataset]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We introduce <em>MEMO</em>, the first public multimodal EMA-OCTA retinal image dataset, and propose <em>VDD-Reg</em>, a deep learning framework that enables robust retinal image registration across large vessel density differences, advancing accurate capillary blood flow measurement for ocular disease diagnosis.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/memo.jpg" alt="MEMO Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="shellcollect">
  <img src="/images/shellcollect.jpg" alt="ShellCollect" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      ShellCollect: A Framework for Smart Precision Shellfish Harvesting Using Data Collection Path Planning
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      Chiao-Yi Wang, ADP Guru Nandhan, <strong>Yi-Ting Shen</strong>, Wei-Yu Chen, Sandip Sharan Senthil Kumar, Alexander Long, Alan Williams, Gudjon Magnusson, Allen Pattillo, Don Webster, Matthew Gray, Miao Yu, and Yang Tao
      <br>
      <em>IEEE Access 2024</em>
      <br>
      <a href="https://ieeexplore.ieee.org/document/10766580">[Paper]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We present <em>ShellCollect</em>, the first smart precision shellfish harvesting framework that plans efficient dredging paths based on underwater oyster distributions, significantly improving harvesting efficiency, and validate its effectiveness through simulation and real-world field tests.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/shellcollect.jpg" alt="ShellCollect Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="ptl">
  <img src="/images/ptl.png" alt="PTL" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      Progressive Transformation Learning for Leveraging Virtual Images in Training
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      <strong>Yi-Ting Shen*</strong>, Hyungtae Lee*, Heesung Kwon, and Shuvra S. Bhattacharyya (* equal contribution)
      <br>
      <em>CVPR 2023</em>
      <br>
      <strong style="color: red;">Selected as a Highlight among the top 10% of accepted papers</strong>
      <br>
      <a href="https://arxiv.org/abs/2211.01778">[arxiv]</a> <a href="https://gitlab.umiacs.umd.edu/dspcad/ptl-release">[Code]</a> <a href="https://www.youtube.com/watch?v=-P1pyGn-1zw&ab_channel=Yi-TingShen">[Video]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We introduce <em>Progressive Transformation Learning (PTL)</em>, a novel framework that progressively transforms and selects virtual UAV images based on domain gap measurements to enhance realism and improve object detection performance, particularly in low-data and cross-domain scenarios.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/ptl.png" alt="PTL Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="archangel">
  <img src="/images/archangel.png" alt="Archangel" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      Archangel: A Hybrid UAV-based Human Detection Benchmark with Position and Pose Metadata
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      <strong>Yi-Ting Shen</strong>, Yaesop Lee, Heesung Kwon, Damon M Conover, Shuvra S. Bhattacharyya, Nikolas Vale, Joshua D Gray, G Jeremy Leong, Kenneth Evensen, and Frank Skirlo
      <br>
      <em>IEEE Access 2023</em>
      <br>
      <a href="https://arxiv.org/abs/2209.00128">[arxiv]</a> <a href="https://ieeexplore.ieee.org/abstract/document/10196325">[Paper]</a> <a href="https://a2i2-archangel.vision/">[Dataset]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We introduce <em>Archangel</em>, the first UAV-based object detection dataset combining real and synthetic data with detailed metadata on UAV position and object pose, enabling precise model diagnosis and providing new insights into learning robust, variation-invariant detection models.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/archangel.png" alt="Archangel Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="ddhc">
  <img src="/images/ddhc.png" alt="DDHC" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      DCT-based Hyperspectral Image Classification on Resource-Constrained Platforms
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      Eung-Joo Lee, <strong>Yi-Ting Shen</strong>, Lei Pan, Zhu Li, and Shuvra S. Bhattacharyya
      <br>
      <em>WHISPERS 2021</em>
      <br>
      <a href="https://ieeexplore.ieee.org/document/9483973">[Paper]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We propose a flexible deep learning framework (<em>DDHC</em>) for hyperspectral image classification that learns from discrete cosine transform (DCT) coefficients, enabling efficient accuracy–computation trade-offs and streamlined deployment on resource-constrained platforms.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/ddhc.png" alt="DDHC Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="depthweak">
  <img src="/images/depthweak.png" alt="DepthWeak" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      What Synthesis is Missing: Depth Adaptation Integrated with Weak Supervision for Indoor Scene Parsing
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      Keng-Chi Liu, <strong>Yi-Ting Shen</strong>, Jan P Klopp, and Liang-Gee Chen
      <br>
      <em>ICCV 2019</em>
      <br>
      <a href="https://arxiv.org/abs/1903.09781">[arxiv]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We propose a novel teacher-student framework for weakly supervised scene parsing that combines synthetic depth-based domain transfer with image-level weak labels via a contour-based integration scheme, significantly narrowing the performance gap to fully supervised methods while reducing annotation effort.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/depthweak.png" alt="DepthWeak Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="deepsortspc">
  <img src="/images/deepsortspc.png" alt="DeepSortSPC" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      Simple Online and Realtime Tracking with Spherical Panoramic Camera
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      Keng-Chi Liu*, <strong>Yi-Ting Shen*</strong>, and Liang-Gee Chen (* equal contribution)
      <br>
      <em>ICCE 2018</em>
      <br>
      <a href="https://ieeexplore.ieee.org/document/8326132">[Paper]</a> <a href="https://github.com/KengChiLiu/MOT360?tab=readme-ov-file">[Dataset]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We propose a simple yet effective real-time multi-object tracking method tailored for 360-degree panoramic videos, achieving significant performance gains over baselines and introducing two new datasets for comprehensive evaluation.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/deepsortspc.png" alt="DeepSortSPC Enlarged" class="enlarged-image">
  </div>
</div>

<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;" id="depthcue">
  <img src="/images/depthcue.png" alt="DepthCue" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      3D Perception Enhancement in Autostereoscopic TV by Depth cue for 3D Model Interaction
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      <strong>Yi-Ting Shen</strong>, Guan-Lin Liu, Sih-Sian Wu, and Liang-Gee Chen
      <br>
      <em>ICCE 2016</em>
      <br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7430613">[Paper]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We present an enhanced autostereoscopic TV system that incorporates Human Visual System-based depth cues to significantly improve 3D perception—doubling viewer depth perception compared to conventional systems—and demonstrate its effectiveness through an interactive 3D model application.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/depthcue.png" alt="DepthCue Enlarged" class="enlarged-image">
  </div>
</div>

Thesis
======
<div style="display: flex; align-items: flex-start; margin-top: 20px; margin-bottom: 20px; position: relative;" id="depthte">
  <img src="/images/depthte.png" alt="DepthTE" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      Self-Supervised Learning of Domain-Specific Depth for Transferable Traversability Estimation with a Single Fisheye Camera
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      <strong>Yi-Ting Shen</strong>
      <br>
      <em>Master Thesis</em>
      <br>
      Advisor: Liang-Gee Chen, Ph.D.
      <br>
      <a href="https://tdr.lib.ntu.edu.tw/handle/123456789/71498?locale=en">[Online]</a> <a href="https://drive.google.com/file/d/1M7YkesgWuoeVZX4T1dj7P1VB3aB0D80T/view?usp=sharing">[Paper]</a> <a href="https://drive.google.com/file/d/1Tse_RuSItM2cUVjQ291Y-icbnumZfE5O/view?usp=sharing">[Report]</a> <a href="https://drive.google.com/file/d/1l8Z7pJ3JbshEKM-AQ2pUdF6Uf4k7hqbz/view?usp=sharing">[Slides]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We propose a two-stage convolutional neural network (<em>D+T-Net</em>) for traversability estimation that leverages domain-specific depth estimation and a universal classifier to achieve high accuracy and strong cross-domain transferability using only a single fisheye camera, making it ideal for real-world, resource-constrained robotic applications.
    </p>
  </div>
  <div class="enlarged-image-container">
    <img src="/images/depthte.png" alt="DepthTE Enlarged" class="enlarged-image">
  </div>
</div>

<style>
/* Add this CSS to your page or a linked stylesheet */
.original-image {
  z-index: 1;
}

.enlarged-image-container {
  display: none;
  position: absolute;
  top: 0;
  left: 170px; /* Adjust to position beside the original image */
  z-index: 10; /* Ensure it appears above other elements */
}

.enlarged-image {
  width: 600px; /* Adjust size for enlargement */
  height: auto;
  border: 2px solid #ccc; /* Optional: Add a border for better visibility */
  background: white; /* Optional: Add a background to avoid overlap issues */
}

.original-image:hover ~ .enlarged-image-container {
  display: block;
}
</style>