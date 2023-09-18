# ARHideNSeeker
Developed alongside: [4019534](https://github.com/4019534)
[Application Demo](https://drive.google.com/file/d/145o6OIQOjJMKoeBDbsqwdSIcQYNOseF2/view?usp=drive_link) 

## Software used
- Unity
- Vuforia Engine

## Description of application
This engaging application offers an immersive gaming experience in the form of a hidden object game. Your objective is to locate a specific image from a given list of objects. To confirm your discovery, simply aim your camera at the sought-after image. And here's the exciting part – successfully uncovering all the hidden images unlocks a well-deserved and rewarding prize!

To bring this delightful concept to life, we harnessed the power of Unity, a versatile and robust platform for creating interactive and visually stunning experiences. Let's delve into the intricacies of how this intriguing application was meticulously crafted.

**User Interface and Transition**:
The journey begins on a user-friendly interface, thoughtfully designed using Unity's fundamental assets. Upon initiating the game by clicking the "Start Game" button, users are seamlessly transported into the world of augmented reality (AR) within the application.

**Visual Clues**:
At the bottom of the screen, six transparent boxes play a pivotal role in guiding the user. These boxes serve as visual cues, hinting at the items that must be located within the area. These item images were meticulously curated and uploaded to the Vuforia portal, subsequently imported into Unity as a custom package. It's worth noting that certain images are intentionally marked as incorrect, and this is cleverly conveyed through a distinctive sound cue reminiscent of the suspenseful sound effects found in popular game shows. In a similar vein, when an image is correctly identified, triggering the corresponding audio cue leads to the satisfying removal of the corresponding box.

**The Rewarding Climax**:
Once all the boxes have been triumphantly removed from the AR landscape, the application notifies the user of their eligibility to claim a delightful "prize." The process involves scanning a designated image displayed on the screen, and upon scanning this image, users are treated to a celebratory video as their well-deserved "prize."

**Image Attribution**:
All the captivating images used in this application have been sourced from the treasure trove of creativity at https://pixabay.com and can be conveniently perused in the images folder thoughtfully included in this repository. For clarity, "Invalid" pertains to images earmarked as incorrect within the context of the game, while "Valid" denotes images confirmed as correct. As for "Prize.jpeg," this intriguing image serves as the gateway to the enchanting celebratory video, marking the culmination of your gaming adventure.

For those eager to embark on this captivating journey, you can access the application by following this link to the APK hosted on Google Drive: [Application APK](https://drive.google.com/file/d/1QstlbPMaCMzK6vKXXzo82rPepMMbly6O/view?usp=drive_link).

Get ready to embrace the challenge, explore the virtual realm, and uncover hidden treasures in this thrilling Unity-based AR adventure!


## Documented code

As this application has been crafted within the Unity environment, its development centers prominently around the aspects of object design and creation, allowing for a streamlined approach to coding. In essence, the project prioritizes the visual and interactive elements, leveraging Unity's powerful tools and capabilities to bring ideas to life with a minimalistic coding footprint. In light of this development approach, I will provide a detailed and thorough step-by-step breakdown of the intricate process that led to the creation of this application, offering insights into how it seamlessly combines the realms of design and functionality within the Unity framework.

### Step 1:
As mentioned earlier, a pivotal step in our application's development journey involved the seamless integration of images from Vuforia into Unity. To achieve this, we first incorporated these images into an image target database within the Vuforia framework. This strategic move not only paved the way for a dynamic and visually compelling experience but also laid the foundation for a harmonious fusion of augmented reality and Unity's capabilities. By creating an image target database, we essentially transformed these images into interactive and context-aware entities within our Unity environment. This step unlocked a plethora of creative possibilities, enabling us to leverage these images as key components in our hidden object game. Each image, now part of the image target database, carried with it a unique significance and potential for engagement within the application. Once these images were seamlessly imported into Unity, they became integral assets in the development process. Unity's intuitive interface allowed us to harness the full potential of these images, weaving them into the fabric of our augmented reality experience. This integration not only streamlined the development process but also enabled us to design captivating interactions and challenges around these images, enhancing the overall gameplay experience. With images from Vuforia expertly integrated into Unity, our application came to life with a captivating blend of augmented reality and immersive gameplay. These images, now imbued with meaning and interactivity, serve as the core elements of our hidden object game. As users embark on their adventure, these images take on a central role, guiding players on a quest to uncover hidden treasures and unlock rewarding surprises. In essence, the process of importing these images from Vuforia into Unity wasn't merely a technical step; it was a creative bridge that connected the real world with the virtual, transforming static images into dynamic, interactive elements that breathe life into our application. This meticulous integration process represents the essence of our development journey, where technology and creativity converge to deliver an unforgettable user experience.


### Step 2:
As the foundation of our augmented reality (AR) adventure took shape, a pivotal realisation emerged: we needed a user interface (UI) to guide and engage our users effectively. This UI would be the bridge between their interactions and the digital world we were creating. To make this happen, we embarked on the journey of UI design and integration, a critical aspect of our application's development. With a clear vision in mind, we began by creating a designated plane within Unity, meticulously tailored to house our UI elements. This plane served as the canvas upon which the user's digital journey would unfold. It provided the perfect backdrop for the seamless integration of Unity's built-in UI elements. One of the key elements of our UI was the "Start Game" interface, strategically positioned to capture the user's attention. Its design was thoughtfully executed to ensure a smooth transition from the interface into the heart of the AR experience. With a simple tap on this plane, users were magically transported into the captivating world of AR, where hidden treasures and challenges awaited their discovery. The heart of the AR experience lay in the AR camera interface, a vital component of our application's design. This interface, while seemingly minimalistic, held the power to guide users on their hidden object quest. At its core, it featured six transparent boxes discreetly positioned along the bottom edge of the screen. These unassuming boxes held the promise of intriguing discoveries, serving as visual cues and markers for the items users needed to locate within the AR environment.

Intriguingly, these seemingly innocuous boxes held the keys to unravelling the mysteries of our augmented reality adventure, and we'll delve deeper into their significance in the unfolding of our narrative. Before we delve further into the intricacies of our AR adventure, it's important to appreciate the thought and effort that went into crafting this intuitive and engaging UI. These elements, meticulously positioned on our UI plane, were the gateway to a world where imagination met technology, and where users could embark on a captivating journey of discovery and rewards.

GUI:


![image](https://github.com/ColemanAlexander/ARHideNSeeker/assets/104588582/c666a9a4-5489-4a5d-90de-cf30acfb062e)


Transparent boxes:


![WhatsApp Image 2023-09-18 at 18 24 46](https://github.com/ColemanAlexander/ARHideNSeeker/assets/104588582/ac556652-cf72-4e82-ad5f-04c0bf5e146f)


### Step 3:
Before we could seamlessly integrate these intriguing images into our user interface, a foundational step was required - the setup of image targets. These image targets were not just static elements; they were the dynamic triggers that would breathe life into our AR experience. By correctly configuring these targets, we ensured that our users would be guided through an engaging and interactive journey. Now, let's explore the intricacies of how we meticulously crafted the "incorrect" image targets. Within Unity's intuitive Inspector panel, we embarked on a journey of customization, tailoring the behaviour of each specific image target to align with the immersive gameplay we envisioned. Here's how we brought these elements to life: 
As we entered the Inspector panel of a specific image target, we ventured into a realm of possibilities. Here, our creative vision merged seamlessly with Unity's functionality.
Within this panel, we embarked on the creation of a specialised function that would become the heart of our "incorrect" image targets. This function was designed to trigger specific actions when the target image was detected by the AR camera.
One of the key actions we encoded within this function was the initiation of an "incorrect" audio cue. When the AR camera successfully identified and locked onto the image target, this audio cue would come to life, creating an audible signal that added depth to the user's experience.
This carefully selected audio cue was reminiscent of those suspenseful game show sound effects, adding an element of excitement and intrigue to the gameplay.
Our innovation didn't stop there. To ensure a seamless and responsive experience, we programmed the function to halt the audio cue once the image target was untracked by the AR camera.
This responsive behaviour added a layer of realism and interactivity to our AR adventure, making users feel truly immersed in the quest for hidden objects.
In essence, the creation of these "incorrect" image targets involved more than just technical configuration. It was a process that melded creativity with precision, with each element carefully orchestrated to enhance the overall user experience. These targets served as not just static markers but as dynamic storytellers, guiding users through a world where hidden treasures and surprises awaited their discovery.

Incorrect image:

![WhatsApp Image 2023-09-18 at 18 24 46 (2)](https://github.com/ColemanAlexander/ARHideNSeeker/assets/104588582/3ceae2c3-cb83-4a9a-8944-85000cfdc908)


Correct Image:

![WhatsApp Image 2023-09-18 at 18 24 47](https://github.com/ColemanAlexander/ARHideNSeeker/assets/104588582/cb12f282-5fa1-41c3-bfa7-903f85e1141a)



### Step 4:
Our journey through the development of this augmented reality (AR) application continues with a closer look at the setup of the image targets for the "correct" images. This aspect of the application followed a similar path to the "incorrect" image targets, yet it introduced a unique twist that added depth and interactivity to the user experience. 
As with the "incorrect" image targets, the "correct" image targets underwent meticulous setup within Unity's Inspector panel. This step was pivotal in ensuring that the user's interactions with these targets would yield meaningful and rewarding outcomes.
What sets the "correct" image targets apart is their mission to render the transparent boxes within the user interface invisible upon detection. Achieving this required a carefully orchestrated sequence of actions, all encapsulated within a function residing within the Inspector panel.
Within this function, a captivating transformation unfolded. The moment the AR camera successfully identified and locked onto a "correct" image target, a series of enchanting actions were set into motion.
The key objective here was to make the transparent boxes, initially serving as visual cues, appear as if they had vanished into thin air. This illusion was achieved by changing their transparency settings, effectively making them invisible while retaining their physical presence on the screen.
The beauty of this interaction lay in its immediacy. Users could witness the transparent boxes seamlessly disappearing as they successfully located and focused on the "correct" image targets, instantly gratifying their efforts and adding a layer of delight to their gameplay. This is achieved through the script Win.c. The script Win.cs, is attached to the Object Canvas (holds all the object text that appears at the bottom of screen). Its function is to check whether all children of the canvas are inactive. If they are then it will activate the Win canvas and the Winner image target. 

#### Win.cs code snippet:

    using UnityEngine;

    public class Win : MonoBehaviour
    {
    public Canvas current, navigateTo;
    public GameObject award;
    public GameObject[] children;
    public bool canvasChildren;

    private void Update()
    {
       
        canvasChildren  = true;

        // foreach (Transform child in current.transform)
        // {
        //     if (child.gameObject.activeSelf)
        //     {
        //         canvasChildren = false;
        //         break; 
        //     }
        // }
        for(int i =0; i<children.Length;i++)
        {
             if (children[i].activeSelf)
            {
                canvasChildren = false;
                break; 
            }
        }



        if (canvasChildren)
        {
            navigateTo.gameObject.SetActive(true);
            award.gameObject.SetActive(true);
        }
    }
}



### Step 5:

In the final and most exciting step of the game, as the user successfully navigates through the challenges and locates all the hidden objects, they eventually reach the winner's canvas. Here, a special winner image target comes into play. When the user scans this image target with their camera, it triggers a captivating sequence. 

Upon scanning the winner image target, the user is gracefully ushered into a dedicated canvas, where they are treated to a celebratory video. This thrilling video serves as the grand finale, bringing their adventurous journey to a satisfying and joyous conclusion. It's the perfect reward for their diligent efforts and successful object-finding skills!

Penultimate screen:


![WhatsApp Image 2023-09-18 at 18 24 45](https://github.com/ColemanAlexander/ARHideNSeeker/assets/104588582/03fd0824-b7fc-459f-a68c-817e2f980de8)



