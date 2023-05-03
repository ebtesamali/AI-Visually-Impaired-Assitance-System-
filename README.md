# AI Visually Impaired Assitance System
AI system for helping visually impaired fully support Arabica language


### Introduction
This project was designed to help visually impaired users navigate their daily routines more easily. We used computer vision and voice recognition techniques to detect and recognize objects that the user needs, such as their phones or kitchen items. Additionally, vocal commands from the user were recognized in Arabic, with responses also generated vocally in Arabic for added convenience. This technology provides a much needed assistive tool for those with visual impairments so they can complete everyday tasks without difficulty or assistance from another person.


the system consists of 3 modules:
* **object detection**
* **speech-to-text**
* **text-to-speech**

![image](https://user-images.githubusercontent.com/67844129/224345124-7212ea32-9658-475c-ab10-d92d24df29b6.png)




### Dataset

In order to complete a project it is essential to have a dataset containing images to localize and detects different items. For this particular project, eight indoor objects were chosen for the datasets. To create these datasets, we scraped images from various sources and then manually annotated them in order to ensure accuracy. Each dataset contains at least 1000 images so that there are enough pictures for accurate results when the model is trained on them. 
Scrapping and annotating thousands of pictures can be time-consuming; however, having such large amounts of data helps improve accuracy during training as well as reduce overfitting due to small sample sizes. This also allows us more flexibility when creating our models since we have plenty of data points that can be used in any combination or arrangement necessary depending on the task at hand. 


 it take extra effort upfront by scraping together all these photos into 8 separate datasets with at least 1000 images each, doing so ensures better performance from our models once they are trained. It also gives us greater control over what type of information goes into making up those sets since everything was collected manually instead relying solely upon automated methods Ultimately this means better end results overall with less time spent dealing with potential issues caused by lack of adequate image samples being available during development stages


The 8 classes that we focused on are as follows:
* **Mobile Phone** 
* **Chair**
*  **Water bottle**
*  **Forks – Sunglasses**
*   **Wallet - Medicine** 
*   **Mugs**

![image](https://user-images.githubusercontent.com/67844129/224348235-81c647fa-bc13-44d2-b306-77a1747b3f24.png)
![image](https://user-images.githubusercontent.com/67844129/224348629-eded1948-b8ef-4abc-bf19-06d57255b262.png)


  ### How does the system works?
  
 The system has two main functionalities which are Discovering and Searching.
* **Discovering mode**: will explore the objects within the camera view and return the
names of the objects that have been detected as an Arabic vocal output.
* **Searching mode**: will receive the name of the object from the user as an Arabic vocal
input, it will search for the object via the user’s camera and return the name of the
object followed by an alarm to notify that the requested object has been found.

![image](https://user-images.githubusercontent.com/67844129/224355007-3af139b8-bf95-40b3-979c-616a3dbce508.png)

1. **Training Data**: The system will identify the 8 classes that we have trained the model
on.
2. **Model**: we used the weight of the model that we have  trained to make the
object detection inference in the system.
3. **Input Data**: We will be using our webcam to feed images at 25 frames per second to
the trained model.
4. **Speech-To-Text API**: for the search mode the system will take a voice input that
specifies the name of the desired object, then send this voice to Google Speech -to-Text
API.
5. **Text-To-Speech API**: The class prediction of the objects detected in every frame will
be string e.g. “cup” we will send this text to the Google Text-to-Speech API using the
gTTS package.
6. **Output**: We will also obtain the coordinates of the bounding box of every object
detected in our frames, overlay the boxes on the objects detected and return the stream
of frames as a video.



 ### Demo
 
