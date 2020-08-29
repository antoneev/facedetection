# Face Detection of Bahamian Athletes
<h2>Classification Problem</h2>

![Image of App Overview]()

I decided to build this program to continue building my knowledge. 

#### Dataset
Images in my dataset were gathered by Google using the Fatkun plugin; however, the downfall with this plugin is you'll have to click download N times for each image you chose. 
In addition, to increase my dataset I used Downloader for Instagram to download bulk images from each athletes Instagram.

#### Data Exploration and Cleaning 
The project uses OpenCV to find the eyes and face of each image. Wavelet is used to give each image depth by breaking the image into segments by feature to give us more information. 
After all images were cropped, in the cropped folder I manually deleted images which were not of the intended athlete. This would happen if the image had multiple individuals within it. 

#### Data Training 
I used GridSearchCV to tune the parameters. I then got the best estimator which in my case was SVM. You'll notice that my model didn't do very good during training or testing, this is expected as the dataset was very small.

Data Visualization of our SVM Model
![Image of Data Visualization]()

#### Backend and Frontend
I then created a Python Flask model to run my model on and connect it to the front-end using HTML which uses CSS and JS to connect the UI and Flask server. 

![Image of Initial App ]()
![Image of App Output]()
