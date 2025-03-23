# stealth-unreal
A starting project with a basic stealth mechanic for Unreal Engine 5


1. INSTALLATION
   - Download the files in the repository.
   - That it.
   - If you want to incorporate the stealth mechanic in a pre-existing the project, the associated files are located:
     - ./Content/Stealth
     - You may need to edit this blueprint to properly detect your player


2. HOW IT WORKS
   - The player enters/exits a sphere radius.
   - Upon entering, a variable in incremented (to a max of 600.)
   - Upon exiting, this same variable is decremented (to a min of 0.)
   - This variable is then divided by 60, which determines enemy behaviour (by default, there are three possible stages.)

3. CUSTOMIZATION
   - Customization is best done by editing the StealthGuy blueprint.
   - Change the amount incremented/decremented & the maximum value (default is 600) to customize how quickly the system becomes "aggressive."
   - Change the value the variable is divided by the customize the amount of phases.
   - Increase the radius of the collision sphere to detect the player from a greater distance.
   - Connect the switch statement at the end of the blueprint to your custom behaviours.


4. IMPORTANT NOTES
   - This project is a 2D sidescroller, if you want to make a different type of game you will need to edit the player controller blueprints and project settings.
   - Enemy AI & assets are not provided, you will need to make those from scratch.
