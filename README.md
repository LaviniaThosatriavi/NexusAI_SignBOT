# Introducing SignBOT by NexusAI
> **Imagine a world without communication barriers between the deaf and the hearing**.

At NexusAI, we strive to address the communication barriers between the hard-of-hearing individuals and those unfamiliar with sign language. We have developed 3 distinct operating features of our application, which is as follows:

## Sign-to-Text Translation
Utilizing OpenCV, TensorFlow Object Detection API, LabelImg, Pre-Trained SSD MobileNet v2 (Transfer Learning), our team developed a Computer Vision-based model that detects hand signals in real-time and converts them to its text equivalence. The current model is trained on a self-engineered dataset consisting of 20 labelled images and 8 testing images for each of hand signals provided. 

*Run Instructions*
1. Navigate to the Tensorflow/scripts directory
2. run ```source venv/bin/activate``` on terminal
3. Navigate to the Tensorflow/models directory
4. run ```export PYTHONPATH=$PYTHONPATH:$PWD```

## Text-to-Sign Translation
Our team made use of OpenCV, Speech Recognition and Natural Language Toolkit to convert text and speech input from the user and output a visual sequence of movements corresponding to the appropriate American Sign Language gesture in the form of a rendered avatar.

*Run Instructions*
1. Make sure both ```Text-to-Sign.ipynb``` and ```assets``` are in the same directory
2. Execute the first cell of the notebook to install necessary modules
3. When prompted, enter ```S``` for speech and ```T``` for text that you would like to be translated
4. For speech, simply say your sentence when ```"Speak Now..."``` is on the screen, the recording will stop once  ```"Converting Speech to Text..."``` appears and the corresponding sentence will be shown.
5. For text, simply enter the sentence in the prompted area

## Chatbot

