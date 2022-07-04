# LS_Detection_Tensorflow ~ Real-time Co-seismic Landslide Detection with Convolutional Neural Networks in Google Colaboratory

For my internship at ITC in Spring 2022 I developed a model that can detect co-seismic landslides nearly in real-time for the area it was trained and tested in, which is the Iburi-Tobu area of Hokkaido, Japan. The model is created using Tensorflow and is based on Sentinel-2 images as wel as the DEM from the SRTM mission. These are freely available in the Google Earth Engine and are retrieved with the code present in: GEE_Images_retrieval.ipynb. The model works very well at a resolution of 10 meter as well as 30 meter, which is visible in the image below.

![Hokkaido_LS_Prediction_1](https://user-images.githubusercontent.com/108480097/177170882-c1d067a0-a5a8-45c0-bdab-3386c6af40b5.jpg)
<i> Image of the landslide detection maps for the Iburi-Tobu area on Hokkaido, Japan at a 10 m resolution (A), 30 m resolution (B) and compared with the validation dataset (C). </i>

To validate the model performance the Receiver Operating Characteristic (ROC) curve and Area Under Curve (AUC) were calculated, which resulted in an ROC curve more inclined to the (1,0) than the 0,0-1,1 comparison line and an AUC value of 0.61 (see the image below).

![Hokkaido_ROC_AUC_1](https://user-images.githubusercontent.com/108480097/177170541-a630ce61-26d1-405c-8dae-31b7bc2822d1.JPG)

<i> Image of the ROC curve and AUC of the Iburi-Tobu area on Hokkaido, Japan. </i>

<b> The code of the model is available in: Landslide_Detection_Tensorflow.ipynb. </b>
