# SiliragungDet

> This repository is documented in Indonesian. Documentation in English will be done as soon as possible.

SiliragungDet merupakan model _object detection_ untuk mendeteksi pemakaian masker (_face mask_). Model ini menggunakan basis model [SSD MobilenetV2 FPNLite 320x320](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md "SSD MobileNet"), ditraining pada dataset [Kaggle Face Mask Detection](https://www.kaggle.com/andrewmvd/face-mask-detection "Kaggle Dataset").

Terdapat dua versi model SiliragungDet, yaitu versi normal dan versi TFLite. Versi TFLite membutuhkan daya komputasi lebih ringan sehingga dapat dijalankan pada perangkat mikrokontroler dan smartphone android.

## Implementasi
------
Implementasi versi TFLite pada perangkat smartphone android dapat dilihat pada [Repository](https://github.com/ruhyadi/SiliragungDet-Android "Repo Android").

Sedangkan, implementasi versi TFLite pada perangkat mikrokontroler (Jetson Nano) dapat dilihat pada [Repository Jetson](https://github.com/ruhyadi "Repo Jetson").

## Notebook
-----
Notebook training, inference dan konversi TFLite dapat dilakukan pada notebook kaggle. 

[![Kaggle Notebook](https://raw.githubusercontent.com/ruhyadi/SiliragungDet-Model/main/Assets/kaggle-notebook.svg)](https://www.kaggle.com/didiruh/siliragungdet-model-training)

## Inference
-----
Inferensi pada notebook

<img src="https://raw.githubusercontent.com/ruhyadi/SiliragungDet-Model/main/Assets/Notebook-1.png"  width="400">

Inferensi pada Android

<img src="https://raw.githubusercontent.com/ruhyadi/SiliragungDet-Model/main/Assets/Android-1.jpeg"  height="400">
<img src="https://raw.githubusercontent.com/ruhyadi/SiliragungDet-Model/main/Assets/Android-3.gif"  height="400">

## Todo
-----
- [x] Training
- [x] TFLite Convertion
- [x] Deploy on Android
- [ ] Quantization
- [ ] Using Haarcascade
  - [ ] Image Classification
