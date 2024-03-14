# Hackathon_wns_trainge
The problem of this hackathon is to classify real damaged cars' images from fake ones. Here is a link to the problem statement https://datahack.analyticsvidhya.com/contest/wns-triange-hackquest/#About

Libraries to work with images:
PIL (pillow): https://pillow.readthedocs.io/en/latest/reference/Image.html

<details>
<summary>Summary of the notebooks: </summary>

The interesting notebook is "hackathon_code". The rest are just draft-ish. </br>
Summary of notebook "Getting to know the images":
All images are RGB and they come in different sizes so we need to resize them.
Keep in mind some nuances when working with images. Simple example, if we read the image using plt.imread, its shape will be HxWxC (C:channels) and its size is the number of pixels. Whereas if we open it with PIL, its size is WxHxC

Notebooks "Padding_cropping_resizing" and "Resizing and saving test images" are self-explanatory.

Summary of notebook "Draft_missing_images_1": I accidentally deleted some images. This notebook is to check which ones and restore them. 

Summary of notebook "Draft_missing_images_2": sanity check that images are complete.

Summary of notebooks "Exploring_Image_augmentation_functions: applying some transformations on the same image. 
</details>

<details>

<summary> Image modification is provided by the modules: </summary>
1. The tf.image module https://www.tensorflow.org/api_docs/python/tf/image/ </br>
2. The module tensorflow.keras.preprocessing.image https://www.tensorflow.org/api_docs/python/tf/keras/preprocessing/image </br>

3. from Keras preprocessing layers: tf.keras.layers
https://keras.io/api/layers/preprocessing_layers/image_augmentation/ <br/>
Example https://www.tensorflow.org/api_docs/python/tf/keras/layers/RandomBrightness

</details>

<details>
<summary> Questions: </summary>
What does each of contrast, hue, saturation, and brightness mean? <br/>
What does tf.image.stateless_random_jpeg_quality do? <br/>
Do noising and blurring reduce the performance of cnns? <br/>
https://forums.fast.ai/t/blur-as-data-augmentation/1385
How to blurr an image? <br/>
https://medium.com/analytics-vidhya/blur-or-change-background-of-images-using-machine-learning-with-tensorflow-f7dab3ddab6f
</details>

<details>
<summary> Helpful Tutorials: </summary>
How to load the images?
TensorFlow Tutorial 18 - Custom Dataset for Images: https://www.youtube.com/watch?v=q7ZuZ8ZOErE&list=PLhhyoLH6IjfxVOdVC1P1L5z5azs0XjMsb&index=18 </br>

Load and preprocess images by tensorflow: https://www.tensorflow.org/tutorials/load_data/images </br>
How to load a custom dataset with images in directories: https://www.youtube.com/watch?v=q7ZuZ8ZOErE&t=1118s </br>

Data augmentation tutorial by tensorflow: https://www.tensorflow.org/tutorials/images/data_augmentation <br/>
Image classification tutorial by tensorflow: https://www.tensorflow.org/tutorials/images/classification </br>

How to Create Efficient Training Pipelines with TensorFlow data.Dataset (Tensorflow Datasets): https://www.youtube.com/watch?v=4WNz2xrGe8w </br>

tf.data: Build TensorFlow input pipelines from tensorflow: https://www.tensorflow.org/guide/data
</details>

<details>
<summary> To read further </summary>
https://keras.io/search.html?query=image%20augmentation
What do Dataset.cache and Dataset.prefetch do? https://www.tensorflow.org/guide/data_performance </br>

</details>



