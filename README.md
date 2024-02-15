# Hackathon_wns_trainge
The problem of this hackathon is to classify real damaged cars' images from fake ones. Here is a link to the problem statement https://datahack.analyticsvidhya.com/contest/wns-triange-hackquest/#About

Libraries to work with images:
PIL (pillow): https://pillow.readthedocs.io/en/latest/reference/Image.html

Summary of notebook "Getting to know the images":
All images are RGB and they come in different sizes so we need to resize them.
Keep in mind some nuances when working with images. Simple example, if we read the image using plt.imread, its shape will be HxWxC (C:channels) and its size is the number of pixels. Whereas if we open it with PIL, its size is WxHxC

Summary of notebook "Padding_cropping_resizing": applying padding and cropping. 
Summary of notebook "Resizing and saving test images" is self-explanatory.

Summary of notebook "Draft_missing_images_1": I accidentally deleted some images. This notebook is to check which ones and restore them. 

Summary of notebook "Draft_missing_images_2": sanity check that images are complete.

Summary of notebooks "Exploring_Image_augmentation_functions: applying some transformations on the same image. 

Image modification is provided by the modules:
1. The tf.image module https://www.tensorflow.org/api_docs/python/tf/image/
2. The module tensorflow.keras.preprocessing.image https://www.tensorflow.org/api_docs/python/tf/keras/preprocessing/image

3. from tf.keras.layers
https://keras.io/api/layers/preprocessing_layers/image_augmentation/ <br/>
Example https://www.tensorflow.org/api_docs/python/tf/keras/layers/RandomBrightness

Data augmentation tutorial by tensorflow: https://www.tensorflow.org/tutorials/images/data_augmentation <br/>
Another relevant tutorial: https://www.tensorflow.org/tutorials/images/classification 

To read further:
https://keras.io/search.html?query=image%20augmentation

Questions: <br/>
What does each of contrast, hue, saturation, and brightness mean? <br/>
What does tf.image.stateless_random_jpeg_quality do? <br/>
Do noising and blurring reduce the performance of cnns? <br/>
https://forums.fast.ai/t/blur-as-data-augmentation/1385
How to blurr an image? <br/>
https://medium.com/analytics-vidhya/blur-or-change-background-of-images-using-machine-learning-with-tensorflow-f7dab3ddab6f

Checking that changing the directory works

