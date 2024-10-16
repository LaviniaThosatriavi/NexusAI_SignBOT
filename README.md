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
5. Navigate back to the original directory
6. run ```jupyter lab```

## Text-to-Sign Translation
Our team made use of OpenCV, Speech Recognition and Natural Language Toolkit to convert text and speech input from the user and output a visual sequence of movements corresponding to the appropriate American Sign Language gesture in the form of a rendered avatar.

*Run Instructions*
1. Make sure both ```Text-to-Sign.ipynb``` and ```assets``` are in the same directory
2. Run all the cells of the notebook. The first cell will download the necessary libraries
3. When prompted, enter ```S``` for speech and ```T``` for text that you would like to be translated
4. For speech, simply say your sentence when ```"Speak Now..."``` is on the screen, the recording will stop once  ```"Converting Speech to Text..."``` appears and the corresponding sentence will be shown.
5. For text, simply enter the sentence in the prompted area

## Chatbot
Using Unsloth, we finetuned Llama-3.1 8b model to create a chatbot feature to help users. It specializes in informations about deafness, the deaf community, ASL, and application guide. It is mainly to assist the user to get more comfortable with the app.

*Run Instructions*
1. As we use Google Colab T4 GPU, instead of running the Jupyter Notebook here, click the link here: [Finetuning Notebook](https://colab.research.google.com/drive/1CIFQQkIGt4aEaCYqOGDwF7tKZ0kVCu-u#scrollTo=yHR5cYjMAG5W)
2. Run all the cell of codes until you reach the cell after training.
3. Test the model in the cell for prompting. Enter your instructions/questions/requests in the "" for instruction. There's a comment showing where it is.

# Conclusion
By employing these three AI-centered solutions within our application, we believe our application could bridge the communication gap between the deaf and the hearing and allow for a more inclusive and sympathetic community. With the integration of more sign and language datasets to our existing models, we are confident that our solution could have a significant and positive impact on our community.
