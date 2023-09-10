# AngryFlappyBird
Implementation of the game Flappy Bird and Angry Bird using JavaFX

Features implemented
---------------------------
1. **Player character:** Avoids all obstacles while collecting as many avocados as possible. A player uses the button to control Koya’s flight. There is a wing flap animation when Koya is flying.
2. **Pipe:** Appears in pairs every fixed amount of time. One life is taken from Koya when a collision with any pipe occurs. Koya bounces backward and drops immediately upon collision.
3. **Bonus object:** Appears randomly on the upward-facing pipes. If a carrot collects an avocado, points are lost. If Koya collects a green avocado, points will be added. If Koya collects a golden avocado, 6 seconds of autopilot mode will be triggered.
4. **Carrot:** Drops randomly from downward-facing pipes and could collect the avocado right beneath it and lead to points lost if the avocado is not collected by Koya first. The game is over, and score is reset to 0 if Koya collides with a carrot. Koya bounces backward and drops immediately upon collision.
5. **Floor:** Scrolls through the scene consistently during the game until a collision happens. The game is over, and score is reset to 0 if Koya collides with the floor. Koya stops moving immediately upon collision.
6. **Background:** Changes from night to day periodically.
7. **UI panel:** UI panel: Provides information about the obstacles and bonus objects, has the button that controls the start of the game and wing flap, and the options for difficulty level selection.
8. **Score:** Points earned are kept track of, and there are three lives that can be lost when Koya runs into a pipe, carrot, or the floor.
9. **Sound effects:** For various events, including getting through pipes, collecting avocados, autopiloting, and hitting an obstacle.


Setup
---------------------------
1. Install Java version 11 or higher.

2. Install JavaFX. 
  * Navigate to https://gluonhq.com/products/javafx/ 
  * Download the compatible version of JavaFX SDK with your Java version. 
  * Unzip the folder and remember its location for later use.
  * If you're using a MAC, follow these extra steps to make sure the computer recognizes the libraries:
    * Navigate to the folder where JavaFX was unzipped. 
    * Go to lib, for each .dylib file 
    * Right-click > Open-with > Terminal > Open and then, close the terminal

3. Download Eclipse.
  * Navigate to the download website: https://www.eclipse.org/downloads/
  * Eclipse Configurations
    * Binding with JAVA:
      * MAC users: Click on Eclipse > Preferences
      * Window users:  Click on Window > Preferences
      * Go to Java > Installed JREs > Choose the one you installed.
      * Execution Environment > JavaSE-11 & Check on compatible JRE
      * Go to Java > Compiler > Set the Compiler Compliance Level to 11 or higher
      * Apply & Close

    * Binding with JavaFX:
      * MAC users: Click on Eclipse > Preferences
      * Window users:  Click on Window > Preferences
      * Go to Java > BuildPath > User Libraries 
      * New > Name “JavaFX11” > Select it and “Add External Jars” > 
      * Find the location where JavaFX (slide 6) was downloaded and select all .jar files.

4. Clone the repository:

   ```bash
   $ git clone https://github.com/MHC-SP23-CS225/angryflappybird-teampocky.git
   ```
   or download as zip and extract.
   
5. Open the repository in Eclipse.
  * Click on File > Import > Projects from Git > Existing Local Repository 
  * Add [Navigate to the local repository's location] > Select [Added repository] > Next > Finish
  * Make sure to follow the Eclipse Configurations to bind with Java and JavaFX in Step 3
    
  
How to play
---------------------------
* The player uses the button to control the Koya’s flight. The Koya is supposed to avoid all obstacles (including pipes, floors and carrots) while collecting as many avocados as possible. 
* If a carrot collects an avocado, 1 point will be lost. If the Koya collects a green avocado, 5 points will be added. If the Koya collects a golden avocado, it will go into autopilot mode and will not collide with any objects.
* If the Koya hits a pipe, 1 point will be lost. If the Koya hits the floor or a carrot, the game is over.
* There are 3 difficulty levels. The harder the game is, the more carrots will appear.


Contributors
---------------------------
* Professor Su (source codes)
* Jennifer Pham
*  Robin Tran

Resources
---------------------------
Images and audios are collected from Google.
