# image_classifier

**Transfer Learning**

We will use the crawler to crop faces and create different image files into a dataset folder.

We have made use of the inception-v3 model trained by google tensorflow researchers.

The model is a Convolutional Neural Network that helps for image recognition.

![Alt text](https://4.bp.blogspot.com/-TMOLlkJBxms/Vt3HQXpE2cI/AAAAAAAAA8E/7X7XRFOY6Xo/s1600/image03.png)

Our goal will not be to build from scratch but use the model to retrain for detecting male or female.

clone the pre-trained ImageNet data set
```
git clone https://github.com/tensorflow/models.git
cd models/tutorials/image/imagenet
python classify_image.py
```
classify_image.py downloads the trained model from google's backend.

![Alt text](https://cdn-images-1.medium.com/max/1200/0*LKl4k_BABDdpAQuV.jpg)

If the model runs correctly, the script will produce the following output:
```
giant panda, panda, panda bear, coon bear, Ailuropoda melanoleuca (score = 0.88493)
indri, indris, Indri indri, Indri brevicaudatus (score = 0.00878)
lesser panda, red panda, panda, bear cat, cat bear, Ailurus fulgens (score = 0.00317)
custard apple (score = 0.00149)
earthstar (score = 0.00127)
```
Clone the flowing url by using this terminal command:
```
git clone https://github.com/koflerm/tensorflow-image-classifier.git
```
Create a directory called:
```
/
--- /training_dataset
|    |
|    --- /Male
|    |    circle1.jpg
|    |    circle_small_red.png
|    |    ...
|    |
|    --- /Female
|         square.jpg
|         square3.jpg
|         ...
```
Use the `train.sh` from the cloned directory to start the retraining process.

Remember that this will allow for 90 % accuracy in prediction which is a good accuracy rate.

After training:
```
python classify.py px0.jpg
```