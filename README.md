# ARHideNSeeker
Developed alongside: 4019534

## Software used
- Unity
- Vuforia Engine

## Description of application
This is a hidden object game where a list of objects are given on the screen and you have to find the corresponding image in the area. Point your camera at the image to verify it is the correct image. Find all the images to get a prize!!!
link to apk in drive: https://drive.google.com/file/d/1QstlbPMaCMzK6vKXXzo82rPepMMbly6O/view?usp=drive_link 

We utilized Unity to develop an AR application that accomplishes the aforementioned tasks. The initial screen features a simple UI design created using Unity's basic assets. Upon clicking the "Start Game" button, the user is seamlessly transitioned to the AR experience within the application.

At the bottom of the screen, six transparent boxes serve as visual cues for the user, indicating the items they need to locate. These item images were first uploaded to the Vuforia portal and subsequently imported into Unity as a custom package. Notably, certain images are designated as incorrect, and this is communicated through a distinctive sound cue reminiscent of a game show sound effect. Similarly, when an image is identified as correct, activating the audio cue results in the corresponding box being removed.

Once all boxes have been successfully removed, the application notifies the user of their eligibility to claim a "prize" by scanning the image displayed on the screen. Upon scanning this image, the user is rewarded with a celebratory video as their "prize."

