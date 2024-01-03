# image Classification
In this data science and machine learning project, we classify sports personalities. We restrict classification to only 5 people,

1.Maria Sharapova
2.Serena Williams
3.Virat Kohli
4.Roger Federer
5.Lionel Messi

Here is the folder structure,

1.UI : This contains ui website code
2.server: Python flask server
3.model: Contains python notebook for model building
4.google_image_scrapping: code to scrap google for images
5.images_dataset: Dataset used for our model training

Technologies used in this project,

1.Python
2.Numpy and OpenCV for data cleaning
3.Matplotlib & Seaborn for data visualization
4.Sklearn for model building
5.Jupyter notebook, visual studio code as IDE
6.Python flask for http server
7.HTML/CSS/Javascript for UI

# DataSet
web scraping to obtain images of specific individuals, namely Maria Sharapova,
Serena Williams, Virat Kohli, Roger Federer, and Lionel Messi, using Google Images. 
Web scraping is a technique where automated tools or scripts are employed to extract information from websites.
code of webscrapping metioned above.

# Methodology for image classifier

# preprocessing : 

(1) Detect eyes and face
Now how do you detect face and eyes?

We will use haar cascade from opencv for this. Here is an article on this:
https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_objdetect/py_face_detection/py_face_detection.html?highlight=haar

(2)  Crop the facial region of the image

(3)  Use wavelet transform as a feature for traning our model

(4)  Now you should have cropped folder under datasets folder that contains cropped images
     Manually examine cropped folder and delete any unwanted images

(5) Images in cropped folder can be used for model training. We will use these raw images along with wavelet transformed images to train our classifier.

 # train the model
 (1) We will use SVM with rbf kernel tuned with heuristic finetuning
 (2) we'll use GridSearch to try out different models with different paramets. Goal is to come up with best modle with best fine tuned parameters
 (3) evaluation of model

 # Frontend









