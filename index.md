## About
I am a PhD student at [Machine Vision Lab](https://balarsgroup.github.io/), IIT Roorkee, where I work under [Prof. R. Balasubramanian](https://sites.google.com/site/balaiitr/) in the field of Computer Vision and Deep Learning. My research interest includes Multimodal Human Activity Recognition using RGB, depth, sensor and infrared data. 

## Research Projects
<table>
  <tr>
    <td><strong>Human action recognition using RGB-D sensor and deep convolutional neural networks</strong></td>
  </tr>
  <tr>
    <td> In this work, we propose an approach to recognize human actions by the fusion of RGB and Depth data. Firstly, Motion History      Images (MHI) are generated from RGB videos which represent the temporal information about the action. Then the original depth data is   rotated in 3D point clouds and three Depth Motion Maps (DMM) are generated over the entire depth sequence corresponding to the front,   side and top projection views. A 4 Channel Deep Convolutional Neural Network is trained, where the first channel is for classifying     MHIs and the remaining three for the front, side and top view generated from depth data respectively. The proposed method is evaluated   on publically available UTD-MHAD dataset which contains both RGB and depth videos. Experimental results show that combining two         modalities gives better recognition accuracy than using each modality individually. 
    </td>
  </tr>
</table>

<table>
  <tr>
    <td><strong>Combining CNN streams of RGB-D and skeletal data for human activity recognition</strong></td>
  </tr>
  <tr>
    <td> Inspired by the success of deep learning methods, for human activity recognition based on individual vision cues, this paper presents a ConvNets based approach for activity recognition by combining multiple vision cues. Moreover, a new method of creating skeleton images, from skeleton joint sequences, representing motion information is presented in this paper. Motion representation images, namely, Motion History Image (MHI), Depth Motion Maps (DMMs) and skeleton images are constructed from RGB, depth and skeletal data of RGB-D sensor. These images are then separately trained on ConvNets and respective softmax scores are fused at the decision level. The combination of these distinct vision cues, leads to complete utilization of data, available from RGB-D sensor. To evaluate the effectiveness of the proposed 5-CNNs approach, we conduct our experiments on three well known and challenging RGB-D datasets, CAD-60, SBU Kinect interaction and UTD-MHAD. Results show that the proposed approach of combining multiple cues by means of decision level fusion is competitive with other state of the art methods. 
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
    <td  style="vertical-align:middle;">Pushpajit Khaire, Praveen Kumar and <b>Javed Imran</b>. "Combining CNN streams of RGB-D and skeletal data for human activity recognition." Pattern         Recognition Letters 115 (2018): 107-116.</td>
  </tr>
  <tr>
    <td><img src="https://i.ibb.co/bFDyz6w/multi-stream-cnn-1.jpg" width="350"/></td>
    <td style="vertical-align:middle;"><b>Javed Imran</b> and Balasubramanian Raman. "Multimodal egocentric activity recognition using multi-stream CNN." ICVGIP (2018).</td>
  </tr>
  <tr>
    <td><img src="https://i.ibb.co/QYYcdLj/0001.jpg" width="350"/></td>
    <td style="vertical-align:middle;"><b>Javed Imran</b> and Balasubramanian Raman. "Evaluating fusion of RGB-D and inertial sensors for multimodal human action recognition."         Journal of Ambient Intelligence and Humanized Computing (2019): 1-20.</td>
  </tr>
</table>
