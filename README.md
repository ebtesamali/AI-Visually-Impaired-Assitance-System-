# AI Visually Impaired Assitance System
AI system for helping visually impaired fully support Arabica language

This project was designed to help visually impaired users navigate their daily routines more easily. We used computer vision and voice recognition techniques to detect and recognize objects that the user needs, such as their phones or kitchen items. Additionally, vocal commands from the user were recognized in Arabic, with responses also generated vocally in Arabic for added convenience. This technology provides a much needed assistive tool for those with visual impairments so they can complete everyday tasks without difficulty or assistance from another person.
the proposed method consists of 3 modules:
* object detection
* speech-to-text
* and text-to-speech.
  ## How does the system works?
  
  The system will first take an audio input from the user, which will be the name of the object that the user is looking for. By using the text-to-speech module the input from this module will be sent to object detection module, and the system will open a real-time camera to find what the user is looking for if the object is in the range of vision of the camera, the system will issue an alert that the object has been found. If the object is not in the range of the camera’s view the system will issue audio to change the camera's position so it can search for the object in another area.
