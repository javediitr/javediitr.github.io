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


<br/>


<table style="width=90%; border: 1px solid black;">
  <tr>
    <td colspan="2"><strong>Deep motion templates and extreme learning machine for sign language recognition</strong></td>
  </tr>
  <tr>
    <td style="text-align: justify;" colspan="3"> <i>Sign Language is a visual language used by persons with hearing and speech impairment to communicate through fingerspellings and body gestures. This paper proposes a framework for automatic sign language recognition without the need of hand segmentation. The proposed method first generates three different types of motion templates: Motion History Image (MHI), Dynamic Image (DI) and our proposed RGB Motion Image (RGBMI). These motion templates are used to ne-tune three ConvNets trained on ImageNet dataset. Fine-tuning avoids learning all the parameters from scratch, leading to faster network convergence even with small number of training samples. For combining the output of three ConvNets, we propose a hybrid late fusion technique based on the combination of traditional feature fusion and score fusion. The features extracted from the last fully connected layer of trained ConvNets are used to train three Kernel based Extreme Learning Machines (KELM), and the nal class label is predicted by averaging their scores. The proposed approach is validated on a number of publicly available sign language as well as human action recognition datasets, and state-of-the-art results are achieved. Finally, an Indian Sign Language (ISL) dataset is also collected using a thermal camera. The experimental results obtained shows that our ConvNet based deep features along with proposed KELM based fusion is robust for any type of human motion recognition.</i>
    </td>
  </tr>    
  <tr align="center">
    <td align="center" style="valign=top; align: center; text-align: justify;" width="50%">
      <img align="middle" src="https://i.ibb.co/mHzJghY/pdfresizer-com-pdf-crop-page-0001.jpg" width="400"/>
      <br/>
      <font size="2">Samples of MHI, DI and RGBMI.</font>
    </td>
    <td align="center" style="valign=top; align: center; text-align: justify;" width="50%">
      <img align="middle" src="https://i.ibb.co/TkvrCPF/arch-page-0001.jpg" width="400"/>
      <br/>
      <font size="2">Proposed three-stream architecture and fusion using KELM.</font>
    </td>
  </tr>
</table>


<br/>


<table style="width=90%; border: 1px solid black;">
  <tr>
    <td colspan="2"><strong>Deep residual infrared action recognition by integrating local and global spatio-temporal cues</strong></td>
  </tr>
  <tr>
    <td style="text-align: justify;" colspan="3"> <i>Human action recognition (HAR) is an important area of research in the field of computer vision. Though a lot of efforts have been made in the past for HAR in visible spectrum, yet progress in infrared domain is still very limited. This is due to the fact that very few infrared action recognition datasets are publicly available, and that too with limited number of classes and training samples. To address this issue, we first construct a new dataset called IITR Infrared Action Recognition (IITR-IAR) dataset with 21 classes, each consisting of 70 samples (total 1470 videos). Then two types of modalities are extracted from each video: Stacked Dense Flow Difference Image (SDFDI) and our newly proposed Stacked Saliency Difference Image (SSDI). Second, we propose a novel four-stream deep framework built upon convolutional neural network (CNN) and recurrent neural network (RNN) models. Our CNN stream is based on deep residual architecture called ResNet, while RNN stream is based on bidirectional long short-term memory (BiLSTM) model. Third, to capture spatio-temporal information at global level, a single SDFDI and a single SSDI are generated using entire video, and then two CNN streams are trained. Similarly to capture spatio-temporal information at local level, a video is divided into eight equal segments, and eight SDFDIs and eight SSDIs are generated. These multiple SDFDIs and SSDIs are then used to train two CNN-BiLSTM streams. Finally, the output of all four streams are combined by late fusion to predict the actual class label. With this four-stream architecture in hand, we achieve state-of-the-art results (83.5%) on InfAR dataset. We also present the baseline result of 75.17% on our proposed IITR-IAR dataset, leaving an ample scope of research for remaining computer vision community to develop and apply more advanced deep learning techniques for infrared HAR.</i>
    </td>
  </tr>    
  <tr align="center">
    <td align="center" style="valign=top; align: center; text-align: justify;" width="50%">
      <img align="middle" src="https://i.ibb.co/qW9tnk9/action-classes-1-page-0001.jpg" width="400"/>
      <font size="2">Samples of IITR-IAR dataset.</font>
    </td>
    <td align="center" style="valign=top; align: center; text-align: justify;" width="50%">
      <img align="middle" src="https://i.ibb.co/3spT23r/4-stream-arch-page-0001.jpg" width="400"/>
      <br/>
      <font size="2">Proposed four-stream architecture.</font>
    </td>
  </tr>
</table>


<table style="width=90%; border: 1px solid black;">
  <tr>
    <td colspan="2"><strong>Robust, efficient and privacy-preserving violent activity recognition in videos</strong></td>
  </tr>
  <tr>
    <td style="text-align: justify;" colspan="3"> <i>Human activity recognition is an extensively researched topic in the field of computer vision. However, some specific events like aggressive behavior or fights have been relatively less investigated. The automatic recognition of such tasks is particularly important in video surveillance scenarios like prisons, railway stations, psychiatric wards, as well as filtering violent contents on-line. In this paper, we attempt to make a violent activity recognition system using deep learning paradigm, which is not only more accurate, but also can be deployed in real-time video surveillance systems. First, multiple approximate dynamic images (ADI) are computed from the input video sequence. An efficient convolutional neural network (CNN) called MobileNet is then used to extract short-term spatio-temporal features from these ADIs. These features are stacked together and fed to a gated recurrent unit (GRU) network, which enables modeling the long-term dynamics of the video sequence. In addition, we also introduce a privacy protection scheme based on randomization of pixel values. The proposed framework is evaluated on three violence recognition benchmark datasets, and the results obtained shows the superiority of our method both in terms of accuracy and memory requirement than the current state-of-the-art.</i>
    </td>
  </tr>    
  <tr align="center">
    <td align="center" style="valign=top; align: center; text-align: justify;" width="50%">
      <img align="middle" src="https://i.ibb.co/Y74ntTY/adi-comparison-page-001.jpg" width="400"/>
      <font size="2">Samples of ADIs generated for high resolution (HR), low resolution (LR) and encrypted (ED) video inputs.</font>
    </td>
    <td align="center" style="valign=top; align: center; text-align: justify;" width="50%">
      <img align="middle" src="https://i.ibb.co/cgM59zQ/arch-page-001.jpg" width="400"/>
      <br/>
      <font size="2">Proposed CNN-GRU architecture.</font>
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
    <td style="vertical-align:middle;"><b>Javed Imran</b> and Balasubramanian Raman. "Deep residual infrared action recognition by integrating local and global spatio-temporal cues."         Infrared Physics & Technology (2019).</td>
  </tr>
  <tr>
    <td><img src="https://i.ibb.co/cgM59zQ/arch-page-001.jpg" width="350"/></td>
    <td style="vertical-align:middle;"><b>Javed Imran</b> and Balasubramanian Raman. "Robust, efficient and privacy-preserving violent    activity recognition in videos ." ACM SAC (2020).</td>
  </tr>
  <tr>
    <td><img src="https://i.ibb.co/309b07G/sasa.jpg" width="350"/></td>
    <td style="vertical-align:middle;">Rahul Kumar, Ridhi Arora, Vipul Bansal, Vinodh J Sahayasheela, Himanshu Buckchash, <b>Javed Imran</b>, Narayanan Narayanan, Ganesh N Pandian and Balasubramanian Raman. "Accurate prediction of covid-19 using chest x-ray images through deep feature learning model with smote and machine learning classifiers." medRxiv (2020).</td>
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
