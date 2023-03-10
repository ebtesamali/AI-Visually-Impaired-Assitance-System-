# AI Visually Impaired Assitance System
AI system for helping visually impaired fully support Arabica language

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
  
  The system will first take an audio input from the user, which will be the name of the object that the user is looking for. By using the text-to-speech module the input from this module will be sent to object detection module, and the system will open a real-time camera to find what the user is looking for if the object is in the range of vision of the camera, the system will issue an alert that the object has been found. If the object is not in the range of the camera’s view the system will issue audio to change the camera's position so it can search for the object in another area.
