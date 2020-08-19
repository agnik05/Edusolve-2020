# TabDrive

## Demo
https://1drv.ms/v/s!AhgwwDStSlSYgoICoVFECmNQlxxhig

## Inspiration
Distracted driving is the biggest contributor to car accidents, a problem that affects over 60 million people annually. By addressing distracted driving, we will save billions of dollars, countless hours of time, and thousands of lives.

## About The Developers
Both Shreeniket and Agnik are high schoolers with a passion for CS.

## What It Does
Our app, DriveSafe, alerts drivers if they are practicing bad driving habits, like reaching backseat, drinking, operating the radio, etc. For best use, the phone should be attached to the car's ventilator using a car vent phone holder. Whenever a driver is doing something unsafe, the app alarts them through a text-to-speech. Our app also has a quiz feature that drivers can take before getting in the car to make sure they're fully sober and not distracted. We also added a feature allowing users to find where their car is in a parking lot using AR, which can also be used by companies like Uber to allow their customers to find their drivers more efficiently. More information can be found in the demo above.

## How We Built It
We used PyTorch and [this dataset from Kaggle](https://www.kaggle.com/c/state-farm-distracted-driver-detection) in order to train a neural network to accurately predict over 10 cases of unsafe driving. Our model achived a 92% valiation over 22,000 images using a pretrained ResNet50 model. We then created an iOS app using Swift and XCode and deployed the model so that it detects these behaviors, which is then articulated by a virtual assistant. This was achieved in real-time by passing every frame of a live video as an image into our neural network. We created the quiz and AR features of the app using Swift, XCode, and echoAR.

## Challenges We Ran Into
Importing the PyTorch model into the format XCode requires was the most difficult and time-consuming part of the project, due to the poor documentation and lack of online resources.

## Accomplishments That We're Proud Of
We're proud of finishing such a complex project in such a short amount of time and hopefully making an impact on the millions of people affected by automobile accidents.

## What We Learned
We learned how to export Tensorflow models to XCode and implement VR tools in iOS apps.

## What's Next For DriveSafe
Hopefully larger distracted driving datasets will be created, so we can retrain our model and classify a wider variety of bad driving habits. We also plan on improving the user interface to make it more aesthetically pleasing for our users.

## Note
Although this repository was created a week ago, we started working on this project on Saturday. Check the commit history for more information. 
