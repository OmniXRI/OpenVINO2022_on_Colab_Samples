# OpenVINO2022_on_Colab_Samples

以下皆是以Intel OpenVINO 2022.3運行於Google Colab環境的範例，主要參考OpenVINO Open Model Zoo Demos 及 Notebooks。

**OpenVINO_Image_Classification_on_Colab.ipynb**   
參考 OpenVINO Notebooks 001-hello-world.ipynb 修改而得，主要可進行Imagenet 1000分類的影像分類。[【Intel官網完整說明】](https://docs.openvino.ai/latest/notebooks/001-hello-world-with-output.html)  
點擊連結可直接運行  
https://colab.research.google.com/github/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/OpenVINO_Image_Classification_on_Colab.ipynb  
![](https://github.com/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/images/image_classification_result_01.jpg)

**OpenVINO_Face_Detection_on_Colab.ipynb**  
參考 OpenVINO Notebooks 004-hello-detection.ipynb 修改而得，主要用於一般物件偵測模型，適用輸出資料結構為 [x_min, y_min, x_max, y_max, conf]。在人臉偵測可適用下列模型，其它模型則由於 output layer 定義不同暫無法使用。[【Intel官網完整說明】](https://docs.openvino.ai/latest/notebooks/004-hello-detection-with-output.html)  

Intel Pre-Trained Model:
* face-detection-0205
* face-detection-0206  

點擊連結可直接運行  
https://colab.research.google.com/github/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/OpenVINO_Face_Detection_on_Colab.ipynb
![](https://github.com/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/images/face_detection_result_01.jpg)  

**OpenVINO_Face_Detection_on_Colab_2.ipynb**  
參考 OpenVINO Notebooks 004-hello-detection.ipynb 修改而得，本程式主要用於一般物件偵測模型，適用輸出資料結構為 [image_id, label, conf, x_min, y_min, x_max, y_max]。在人臉偵測可適用下列模型，其它模型則由於 output layer 定義不同暫無法使用。[【Intel官網完整說明】](https://docs.openvino.ai/latest/notebooks/004-hello-detection-with-output.html)  

Intel Pre-Trained Model:  
* face-detection-0200
* face-detection-0202
* face-detection-adas-0001
* face-detection-retail-0004
* face-detection-retail-0005  

Public Pre-Trained Model:  
* face-detection-retail-0044  

點擊連結可直接運行  
https://colab.research.google.com/github/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/OpenVINO_Face_Detection_on_Colab_2.ipynb
![](https://github.com/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/images/face_detection_result_01.jpg)  

**OpenVINO_Segmentation_(ADAS)_on_Colab.ipynb**  
參考 OpenVINO Notebooks 003-hello-segmentation.ipynb 修改而得。本程式主要用於一般影像（語義）分割模型， 適用輸入資料結構為 [B, C, H, W] （1, 3, 512, 896)，輸出資料結構為 [B, C, H, W] (1, 4, 512, 896)，其輸出分類為 BG, Road, Curbs, Marks四類，並以顏色區隔。目前僅支援 road-segmentation-adas-0001 影像（語義）分割模型，其它模型則由於 output layer 定義不同暫無法使用。[【Intel官網完整說明】](https://docs.openvino.ai/latest/notebooks/003-hello-segmentation-with-output.html)  

點擊連結可直接運行   
https://colab.research.google.com/github/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/OpenVINO_Segmentation_(ADAS)_on_Colab.ipynb
![](https://github.com/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/images/segmentation(ADAS)_result_01.jpg)  

**OpenVINO_Pose_Estimation_on_Colab.ipynb**  
參考 OpenVINO Notebooks 402-pose-estimation.ipynb 改寫，本程式主要用於一般姿態估測模型，採COCO定義之18個關鍵點，輸入影像結構為 [B, C, H, W] （1, 3, 256, 456)，輸出為 Mconv7_stage2_L1（1, 38, 32, 57）及Mconv7_stage2_L2（1, 19, 32, 57）。 目前僅支援 human-pose-estimation-0001 ，其它模型則由於 output layer 定義不同暫無法使用。  
原範例可支援網路攝影機，但這裡僅示範使用影片檔案輸入。[【Intel官網完整說明】](https://docs.openvino.ai/latest/notebooks/402-pose-estimation-with-output.html)  

點擊連結可直接運行  
https://colab.research.google.com/github/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/OpenVINO_Pose_Estimation_on_Colab.ipynb
![](https://github.com/OmniXRI/OpenVINO2022_on_Colab_Samples/blob/main/images/pose_estimation_result_01.jpg)  
