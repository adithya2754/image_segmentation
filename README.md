# Image Segmentation with U-Net

This type of image classification is called semantic image segmentation. It's similar to object detection in that both ask the question: "What objects are in this image and where in the image are those objects located?," but where object detection labels objects with bounding boxes that may include pixels that aren't part of the object, semantic image segmentation allows you to predict a precise mask for each object in the image by labeling each pixel in the image with its corresponding class. The word “semantic” here refers to what's being shown, so for example the “Car” class is indicated below by the dark blue mask, and "Person" is indicated with a red mask:

<img src="images/carseg.png" style="width:500px;height:250;">
<caption><center> <u><b>Figure 1</u></b>: Example of a segmented image <br> </center></caption>


As you might imagine, region-specific labeling is a pretty crucial consideration for self-driving cars, which require a pixel-perfect understanding of their environment so they can change lanes and avoid other cars, or any number of traffic obstacles that can put peoples' lives in danger.

Key Take-overs of the project:
* Building a U-Net
* Explain the difference between a regular CNN and a U-net
* Training the model using Adam optimizer on the CARLA self-driving car data-set of 1000+ images
* Implementing semantic image segmentation on the CARLA self-driving car dataset
* Applying sparse categorical crossentropy for pixelwise prediction


Outputs using 40 epochs:

![image](https://user-images.githubusercontent.com/96827791/211162923-831e6194-57e1-47b9-9fc9-2946187c66a4.png)
![image](https://user-images.githubusercontent.com/96827791/211162960-bbef4556-2435-43a1-b583-f87138b11bd4.png)
![image](https://user-images.githubusercontent.com/96827791/211162962-d1830274-2709-4f2b-aba9-e9c4d7f7b62c.png)
![image](https://user-images.githubusercontent.com/96827791/211162968-6f1780fc-16af-499f-b7c7-319eba90cbff.png)

