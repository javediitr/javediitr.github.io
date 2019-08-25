## About
I am a PhD student at [Machine Vision Lab](https://balarsgroup.github.io/), IIT Roorkee, where I work under [Prof. R. Balasubramanian](https://sites.google.com/site/balaiitr/) in the field of Computer Vision and Deep Learning. My research interest includes Multimodal Human Activity Recognition using RGB, depth, sensor and infrared data. 

## Research Projects
<table>
  <tr>
    <td><strong>Human action recognition using RGB-D sensor and deep convolutional neural networks</strong></td>
  </tr>
  <tr>
    <td style="text-align: justify;"> In this work, we propose an approach to recognize human actions by the fusion of RGB and Depth data. Firstly, Motion History Images (MHI) are generated from RGB videos which represent the temporal information about the action. Then the original depth data is rotated in 3D point clouds and three Depth Motion Maps (DMM) are generated over the entire depth sequence corresponding to the front, side and top projection views. A 4-Channel Deep Convolutional Neural Network is trained, where the first channel is for classifying MHIs and the remaining three for the front, side and top view generated from depth data respectively. The proposed method is evaluated on publically available UTD-MHAD dataset which contains both RGB and depth videos. Experimental results show that combining two modalities gives better recognition accuracy than using each modality individually. 
    </td>
  </tr>
</table>

<br/>

<table>
  <tr>
    <td><strong>Combining CNN streams of RGB-D and skeletal data for human activity recognition</strong></td>
  </tr>
  <tr>
    <td style="text-align: justify;"> Inspired by the success of deep learning methods, for human activity recognition based on individual vision cues, this paper presents a ConvNets based approach for activity recognition by combining multiple vision cues. Moreover, a new method of creating skeleton images, from skeleton joint sequences, representing motion information is presented in this paper. Motion representation images, namely, Motion History Image (MHI), Depth Motion Maps (DMMs) and skeleton images are constructed from RGB, depth and skeletal data of RGB-D sensor. These images are then separately trained on ConvNets and respective softmax scores are fused at the decision level. The combination of these distinct vision cues, leads to complete utilization of data, available from RGB-D sensor. To evaluate the effectiveness of the proposed 5-CNNs approach, we conduct our experiments on three well known and challenging RGB-D datasets, CAD-60, SBU Kinect interaction and UTD-MHAD. Results show that the proposed approach of combining multiple cues by means of decision level fusion is competitive with other state of the art methods. 
    </td>
  </tr>
</table>

<br/>

<table style="width=90%; border: 1px solid black;">
  <tr>
    <td colspan="3"><strong>Multimodal egocentric activity recognition using multi-stream CNN</strong></td>
  </tr>
  <tr>
    <td style="text-align: justify;" colspan="3"> <i>Egocentric activity recognition (EAR) is an emerging area in the field of computer vision research. Motivated by the current success of Convolutional Neural Network (CNN), we propose a multistream CNN for multimodal egocentric activity recognition using
visual (RGB videos) and sensor stream (accelerometer, gyroscope, etc.). In order to effectively capture the spatio-temporal information
contained in RGB videos, two types of modalities are extracted from visual data: Approximate Dynamic Image (ADI) and Stacked Difference Image (SDI). These image-based representations are generated both at clip level as well as entire video level, and are then utilized to finetune a pretrained 2D-CNN called MobileNet, which is specifically designed for mobile vision applications. Similarly for sensor data, each training sample is divided into three segments, and a deep 1D-CNN network is trained (corresponding to each type of sensor stream) from scratch. During testing, the softmax scores of all the streams (visual + sensor) are combined by late fusion. The experiments performed on multimodal egocentric activity dataset demonstrates that our proposed approach can achieve state-of-the art results, outperforming the current best handcrafted and deep learning based techniques.</i>
    </td>
  </tr>    
  <tr>
    <td style="valign=top; text-align: justify;" width="33%">
      <img src="https://i.ibb.co/tMDJvzN/visual-1.jpg" width="250"/>
      <br/>
      <font size="2">Generation of ADIs and SDIs for visual stream. Each video sample is divided into 3 equal segments (without overlapping), and then four ADIs and four SDIs are generated (three at clip-level and one at entire video level).</font>
    </td>
    <td style="valign=top; text-align: justify;" width="33%">
      <img src="https://i.ibb.co/tpHhdYC/sensor-1.jpg" width="250"/>
      <br/>
      <font size="2">Illustration of preprocessing done for sensor stream. Each input sample is divided three equal segments: Segment 1 (1-100), Segment 2 (26-125), Segment 3 (51-150).</font>
    </td>
    <td style="valign=top; text-align: middle;" width="34%">
      <img src="https://i.ibb.co/bFDyz6w/multi-stream-cnn-1.jpg" width="300"/>
      <br/>
      <font size="2">Proposed multi-stream CNN.</font>
    </td>
  </tr>
</table>

<br/>





<table style="width=90%; border: 1px solid black;">
  <tr>
    <td colspan="3"><strong>Evaluating fusion of RGB-D and inertial sensors for multimodal human action recognition</strong></td>
  </tr>
  <tr>
    <td style="text-align: justify;" colspan="3"> <i>Fusion of multiple modalities from different sensors is an important area of research for multimodal human action recognition. In this paper, we conduct an in-depth study to investigate the effect of different parameters like input preprocessing, data augmentation, network architectures and model fusion so as to come up with a practical guideline for multimodal action recognition using deep learning paradigm. First, for RGB videos, we propose a novel image-based descriptor called stacked dense flow difference image (SDFDI), capable of capturing the spatio-temporal information present in a video sequence. A variety of deep 2D convolutional neural networks (CNN) are then trained to compare our SDFDI against state-of-the-art
image-based representations. Second, for skeleton stream, we propose data augmentation technique based on 3D transformations so as to facilitate training a deep neural network on small datasets. We also propose a bidirectional gated recurrent unit (BiGRU) based recurrent neural network (RNN) to model skeleton data. Third, for inertial sensor data, we propose data augmentation based on jittering with white Gaussian noise along with deep a 1D-CNN network for action classification. The outputs of all these three heterogeneous networks (1D-CNN, 2D-CNN and BiGRU) are combined by a variety of model fusion approach based on score and feature fusion. Finally, in order to illustrate the efficacy of the proposed framework, we test our model on a publicly available UTD-MHAD dataset, and achieved an overall accuracy of 97.91%, which is about 4% higher than using each modality individually. We hope that the discussions and conclusions from this work will provide a deeper insight to the researchers in the related fields, and provide avenues for further studies for different multi-sensor based fusion architectures.</i>
    </td>
  </tr>    
  <tr>
    <td style="valign=top; align: center; text-align: justify;" width="40%">
      <img src="https://i.ibb.co/Fn9ZR7C/Figure5-1.jpg" width="330"/>
      <br/>
      <font size="2">Comparison of proposed SDFDI against other state-of-the-art image-based representations.</font>
    </td>
    <td style="valign=top; align: center; text-align: justify;" width="23%">
      <img src="https://i.ibb.co/GTNV8Mj/Figure7b-1.jpg" width="250"/>
      <br/>
      <font size="2">Data augmentation of inertial stream using signal jittering.</font>
    </td>
    <td style="valign=top; align: center; text-align: middle;" width="37%">
      <img src="https://i.ibb.co/QYYcdLj/0001.jpg" width="290"/>
      <br/>
      <font size="2">Proposed multimodal architecture.</font>
    </td>
  </tr>
</table>

## Publications

<table>
  <tr valign="middle">
    <td><img src="https://i.ibb.co/vsw9cgw/Untitled.png" width="350"/></td>
    <td style="vertical-align:middle;"><strong>Javed Imran</strong> and Praveen Kumar. "Human action recognition using RGB-D sensor and deep convolutional neural networks." ICACCI (2016)     </td>
  </tr>
  <tr valign="middle">
    <td><img src="https://i.ibb.co/nzjcMK2/Untitled.png" width="350"/></td>
    <td  style="vertical-align:middle;">Pushpajit Khaire, Praveen Kumar and <b>Javed Imran</b>. "Combining CNN streams of RGB-D and skeletal data for human activity recognition." Pattern Recognition Letters 115 (2018): 107-116.</td>
  </tr>
  <tr>
    <td><img src="https://i.ibb.co/bFDyz6w/multi-stream-cnn-1.jpg" width="350"/></td>
    <td style="vertical-align:middle;"><b>Javed Imran</b> and Balasubramanian Raman. "Multimodal egocentric activity recognition using multi-stream CNN." ICVGIP (2018).</td>
  </tr>
  <tr>
    <td><img src="https://i.ibb.co/QYYcdLj/0001.jpg" width="350"/></td>
    <td style="vertical-align:middle;"><b>Javed Imran</b> and Balasubramanian Raman. "Evaluating fusion of RGB-D and inertial sensors for multimodal human action recognition."         Journal of Ambient Intelligence and Humanized Computing (2019): 1-20.</td>
  </tr>
  <tr>
    <td><img src="https://i.ibb.co/TkvrCPF/arch-page-0001.jpg" width="350"/></td>
    <td style="vertical-align:middle;"><b>Javed Imran</b> and Balasubramanian Raman. "Deep motion templates and extreme learning machine for sign language recognition."         The Visual Computer (2019): 1-14.</td>
  </tr>
  <tr>
    <td><img src="https://i.ibb.co/3spT23r/4-stream-arch-page-0001.jpg" width="350"/></td>
    <td style="vertical-align:middle;"><b>Javed Imran</b> and Balasubramanian Raman. "Deep Residual Infrared Action Recognition by Integrating Local and Global Spatio-Temporal Cues."         Infrared Physics & Technology (2019).</td>
  </tr>
</table>


## Awards and Scholarships
<ol>
  <li>GATE 2014 and 2016 qualified.</li>
  <li>NET 2014 qualified.</li>
  <li>M.Tech Gold Medalist (9.8 CGPA)</li>
  <li>Senator of Student Gymkhana for M.Tech batch</li>
  <li>4 years of teaching experience as a Computer Science faculty.</li>
</ol>
