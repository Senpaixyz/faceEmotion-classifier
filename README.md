# FaceEmotion Classifier 

The face emotion classifier web application developed in this study can accurately predict seven distinct types of emotions. The model was built using convolutional neural networks (CNN) with layers configured to accept input of size (48, 48, 1), denoting grayscale images with dimensions of 48x48 pixels. Training the model took 50 epochs, a measure of how many times the entire training dataset was passed forward and backward through the neural network. During testing, the model achieved an accuracy rate of 85%, indicating its effectiveness in accurately classifying emotions based on input images. The application itself is deployed using Flask as the backend server and is hosted on Heroku, providing users with a reliable and accessible platform for emotion recognition tasks.

[![N|Solid](https://github.com/Senpaixyz/faceEmotion-classifier/blob/master/images/landing%20page.PNG?raw=true)](https://github.com/Senpaixyz/faceEmotion-classifier/blob/master/images/landing%20page.PNG)

## Features

- The predictor model can predict multiple faces in a single frame.
- It  has 82% accuracy so it is good enough for prediction.
- It can be deployed in realtime or be use as API.
- Soon to add realtime face emotion classifier via Flask Web App.

## Instruction

- The image that will upload must be 500x500 pixels or higher
- It must be a valid image file.
- The image must contain human face/s else the predictor will return None.
- Drag and drop markdown and HTML files into Dillinger
- The size of the image must be less than 2mb.

This face emotion classifier web application can predict 7 types of emotions. To produce a model the study build a convolutional neural networks layers with (48,48,1) input shape and 50 epochs. The accuracy of the model got 85% in testing.

### Datasets

I downloaded the [datasets](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data) that Ive use in this web application from the Kaggle. It consist of 48x48 pixels grayscale images of faces. Each classes was identified.

| Key Index | Type of Emotion |
| ------ | ------ |
| 0 | ANGRY |
| 1 | DISGUST|
| 2 | FEAR |
| 3 | HAPPY |
| 4 | SAD |
| 5 | SURPRISE |
| 6 | NEUTRAL |

### Predictor

The sample UI of face emotion classifier web application after the user uploaded the image.

[![N|Solid](https://github.com/Senpaixyz/faceEmotion-classifier/blob/master/images/predicted.PNG?raw=true)](https://github.com/Senpaixyz/faceEmotion-classifier/blob/master/images/predicted.PNG)

The predictor model will tell you how accurate that the prediction was. Since it is not perfect there are some instances that the predictor model will predict incorrect emotion.

[![N|Solid](https://github.com/Senpaixyz/faceEmotion-classifier/blob/master/images/accuracy.PNG?raw=true)](https://github.com/Senpaixyz/faceEmotion-classifier/blob/master/images/accuracy.PNG)

#### Installation

For first time use, please create virtual environment from the Pycharm IDE. Then open the terminal and run:

```sh
pip install -r requirements.txt
```
After use install all the dependency that needed in this web application. just simply type in the terminal:

```sh
python app.py
```
Verify the deployment by navigating to your server address in
your preferred browser.

```sh
http://127.0.0.1:5000/
```
This web application was supported by ngrok api. Uncomment this in the app.py to use it and shared this web application from another devices and via internet.

`//run_with_ngrok(app)`

## License

MIT

**Free Web Application Developed by Jheno Cerbito**
