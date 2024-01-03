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

1.preprocessing : Detect eyes and face

When we look at any image, most of the time we identify a person using a face.
An image might contain multiple faces, also the face can be obstructed and not clear.
The first step in our pre-processing pipeline is to detect faces from an image. 
Once face is detected, we will detect eyes, if two eyes are detected then only we keep that image otherwise discard it.

Now how do you detect face and eyes?

We will use haar cascade from opencv for this. Here is an article on this:
https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_objdetect/py_face_detection/py_face_detection.html?highlight=haar
