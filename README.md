# ARHideNSeeker
Developed alongside: [4019534](https://github.com/4019534)

## Software used
- Unity
- Vuforia Engine

## Description of application
This is a hidden object game where a list of objects is presented on the screen, and your task is to locate the matching image within the environment. To confirm its correctness, simply aim your camera at the image. Discovering all the images unlocks a rewarding prize!
link to apk in drive: https://drive.google.com/file/d/1QstlbPMaCMzK6vKXXzo82rPepMMbly6O/view?usp=drive_link 

We utilized Unity to develop an AR application that accomplishes the aforementioned tasks. The initial screen features a simple UI design created using Unity's basic assets. Upon clicking the "Start Game" button, the user is seamlessly transitioned to the AR experience within the application.

At the bottom of the screen, six transparent boxes serve as visual cues for the user, indicating the items they need to locate. These item images were first uploaded to the Vuforia portal and subsequently imported into Unity as a custom package. Notably, certain images are designated as incorrect, and this is communicated through a distinctive sound cue reminiscent of a game show sound effect. Similarly, when an image is identified as correct, activating the audio cue results in the corresponding box being removed.

Once all boxes have been successfully removed, the application notifies the user of their eligibility to claim a "prize" by scanning the image displayed on the screen. Upon scanning this image, the user is rewarded with a celebratory video as their "prize."

All images were obtained from https://pixabay.com and can be viewed in the images folder included in this repository. Invalid refers to images marked as incorrect within the context of the game. Valid refer to the images marked as correct. Prize.jpeg is the image that leads to the celebratory video.


## Documented code

As this application has been crafted within the Unity environment, its development centers prominently around the aspects of object design and creation, allowing for a streamlined approach to coding. In essence, the project prioritizes the visual and interactive elements, leveraging Unity's powerful tools and capabilities to bring ideas to life with a minimalistic coding footprint. In light of this development approach, I will provide a detailed and thorough step-by-step breakdown of the intricate process that led to the creation of this application, offering insights into how it seamlessly combines the realms of design and functionality within the Unity framework.

