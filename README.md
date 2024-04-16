# Space invader test

## Target - 
To find all the bugs and enable the game to run 

#### Part 1 - Setting up your Project 
    - Executed in approx **15** minutes.
    - In this part I was supposed to setup my project. 
    - Firstly, I was supposed to fork and clone the repository to my local device. https://github.com/outscal/SME-Assignment
    Then the next step was to add the SFML 2.6.1 files to my project following the setup guide.

#### Part 2 - Bug Fixing
    - Executed in approx **10** minutes.
    - In this step, I had to find a deliberate bug in the code, that was preventing the game to run. 
    - The bug was in space invasion -> header -> Player -> PlayerController.h
    -To solve the bug we just had to define the two class **"class PlayerModel; " and "class PlayerView;"**. 
    -This was done because the file was accesssing these two classes without definiing them in the file.

#### Part 3 – Small Improvements 
    - Executed in approx 1 hour.
    - spent approximately 2hour on further research and exploration.
    - In this step, I was supposed to add the processBuletfire() function to the PLayerController.cpp
    - The Event Left mouse Click demands a bullet fire.
    - A function processBulletFire() was defined under PlayerController.h file and Playercontroller.cpp
    - This functions calls the spawnParticleSystem() function in the ParticleSystem. 
    - This initialises the Bullet at the starting point (that is the current location of the player).
    - A Bullet fire sound effect was called from the Global -> ServiceLocator.cpp.

    - There are few more modifications that can be done in this function. 
    - A Bullets vector defined to store every bullent rendering location. 
    - A boundary condition to check if the Bullet rendering location is out of Bound then it will pop that
      location out of the Vector. 
    - A if-else condition to check for the powerup type and call the required powerup accordingly.


