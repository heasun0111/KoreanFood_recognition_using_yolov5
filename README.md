# KoreanFood recognition using yolov5
<br>

This project was conducted in the fall semester of 2021 as a UNLV internship project. And this project is a personal project with feedback from the professor (Dr. Morrison). We trained the YOLOv5 model using UEC_FOOD_256 data and Korean food data. <br>
Details of the data and model can be found at the link below. <br>
[YOLOv5](https://github.com/ultralytics/yolov5)<br>
[UEC_FOOD_256](http://foodcam.mobi/dataset256.html)<br>
[Korean food data](https://github.com/heasun0111/KoreanFood-Recognition)<br> <br>

<p align="center"><img src="./img/ppt.png" width="800" heigth="600"/></p> 
Hello, I'm Hyesun Hong. I am a student at Korea Aerospace University in Korea. <br>
My major is Computer Science, and I am currently a senior. I came to UNLV in the fall semester of 2021 and worked on the Food Recognition project using YOLOv5. Then I'll start the presentation of the project I've been working on this semester. <br> <br> <br>

<p align="center"><img src="./img/ppt2.png" width="800" heigth="600"/></p>
This is the contents, and each part contains the following information.
<br> <br> <br>

<p align="center"><img src="./img/ppt3.png" width="800" heigth="600"/></p>
Diet has a lot of influence on health. Bad eating habits cause many diseases And healthy diets make a balanced body. <br>
Recently, many people use their cell phones to keep a diet journal. <br>
Then, what if there is a program that automatically labels food from photos And analyzes the diet? <br>
<br> <br> <br>

<p align="center"><img src="./img/ppt40.png" width="800" heigth="600"/></p>
More convenient usage will make it easier for many people to control their diet, save time and increase accessibility.<br>
In anticipation of these benefits, the food recognition project began. We trained UEC_FOOD_256 data and Korean food data on yolov5, and measured the accuracy of the model through precision, recall, and mAP.
<br> <br> <br>

<p align="center"><img src="./img/ppt4.png" width="800" heigth="600"/></p>
The settings for this project are as follows. <br>
Use MobaXterm to remotely connect to the AI server. And build a virtual environment using miniconda. Miniconda makes it easy to create multiple virtual environments and to install libraries needed for projects. Machine learning training takes a lot of time, but if the session is disconnected, training will be stopped. To solve this problem, use tmux to multiplex the console so that training continues even when the session is closed.
<br> <br> <br>

<p align="center"><img src="./img/ppt5.png" width="800" heigth="600"/></p>
The datasets are as follows. <br>
There are two types of data, UEC_FOOD_256 data and Korean Food data. The UEC_FOOD_256 dataset consists of 256 kinds of Japanese food and other countries' food, with 100~600 images per category. This dataset is open-source and could be used without any special conditions. However, the format of UEC_FOOD_256 bounding box and the format of YOLOv5 were different. So conversion was required. We used the ‘food_generate_bbox_file.py’ and ‘food_split_for_yolo.py’ codes found to a format suitable for YOLOv5.
<br> <br> <br>

<p align="center"><img src="./img/ppt6.png" width="800" heigth="600"/></p>
And the Korean food dataset is made by using Roboflow. <br>
We divided upper categories such as rice/soup/noodles/meat side dishes/vegetables side dishes/fish side dishes/kimchi. And there are 53 subcategories, and the data have 100~150 images per category.
<br> <br> <br>

<p align="center"><img src="./img/ppt7.png" width="800" heigth="600"/></p>
The collected images were created and labeled using roboflow, and data augmentation was used to increase insufficient data. Using data augmentation, we can increase 600 images to 2,400.
<br> <br> <br>

<p align="center"><img src="./img/ppt8.png" width="800" heigth="600"/></p> <br> <br>
<p align="center"><img src="./img/ppt9.png" width="800" heigth="600"/></p> <br> <br>
<p align="center"><img src="./img/ppt10.png" width="800" heigth="600"/></p> <br> <br>
<p align="center"><img src="./img/ppt11.png" width="800" heigth="600"/></p> <br> <br>
<p align="center"><img src="./img/ppt12.png" width="800" heigth="600"/></p> <br> <br>
<p align="center"><img src="./img/ppt13.png" width="800" heigth="600"/></p> <br> <br>
<br>
We welcome all opinions such as code and README grammar,<br>
so if you find any problems, please feel free to contact us.<br>
