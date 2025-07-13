# Flower Image Classification with CNN

Proyek ini adalah implementasi model Convolutional Neural Network (CNN) untuk mengklasifikasikan gambar bunga ke dalam beberapa kelas: daisy, dandelion, rose, sunflower, tulip.

## Struktur Proyek

submission
├───tfjs_model
| ├───group1-shard1of1.bin
| └───model.json
├───tflite
| ├───model.tflite
| └───label.txt
├───saved_model
| ├───saved_model.pb
| └───variables
├───notebook.ipynb
├───README.md
└───requirements.txt

## Dataset

https://www.kaggle.com/datasets/lara311/flowers-five-classes
Dataset yang digunakan adalah kumpulan gambar bunga dengan 2696 gambar yang saya pakai yang terbagi menjadi 3 kelas:
- daisy
- dandelion
- rose
- sunflower
- tulip


## Model

Model CNN dibuat menggunakan TensorFlow/Keras dengan arsitektur Sequential dan transfer learning MobileNetV2. Model dilatih hingga mencapai akurasi Akurasi Training Set: 94.54% dan Akurasi Testing Set: 89.63%.

## Format Ekspor Model

Model diekspor ke:
- SavedModel
- TFLite
- TensorFlow.js

## Label

File `label.txt` berisi daftar nama kelas:
- daisy
- dandelion
- rose
- sunflower
- tulip