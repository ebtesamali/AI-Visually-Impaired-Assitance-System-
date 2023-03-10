# AI Visually Impaired Assitance System
AI system for helping visually impaired fully support Arabica language

in this project, we  used computer vision and voice recognition techniques to guide visually impaired users to find the objects they need during their daily routines via object detection and recognition. Vocal user commands and responses are also generated vocally in Arabic. 
the proposed method consists of 3 modules:
* object detection
* speech-to-text
* and text-to-speech.
  ## How does the system works?
  
  The system will first take an audio input from the user, which will be the name of the object that the user is looking for. By using the text-to-speech module the input from this module will be sent to object detection module, and the system will open a real-time camera to find what the user is looking for if the object is in the range of vision of the camera, the system will issue an alert that the object has been found. If the object is not in the range of the camera’s view the system will issue audio to change the camera's position so it can search for the object in another area.
