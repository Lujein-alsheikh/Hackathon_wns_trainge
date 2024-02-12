# Hackathon_wns_trainge
The problem of this hackathon is to classify real damaged cars' images from fake ones. Here is a link to the problem statement https://datahack.analyticsvidhya.com/contest/wns-triange-hackquest/#About

Libraries to work with images:
PIL (pillow): https://pillow.readthedocs.io/en/latest/reference/Image.html

Summary of notebook "Getting to know the images":
All images are RGB and they come in different sizes so we need to resize them.
Keep in mind some nuances when working with images. Simple example, if we read the image using plt.imread, its shape will be HxWxC (C:channels) and its size is the number of pixels. Whereas if we open it with PIL, its size is WxHxC

Summary of notebook "Resizing and saving test images":
Resizing the test images and saving them. 
