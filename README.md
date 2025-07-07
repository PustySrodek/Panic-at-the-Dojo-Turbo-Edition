# Panic at the Dojo: Turbo Edition
### Requirements to run this project:
- Unreal Engine 5.4.4

The entire project is made in Blueprints Visual Scripting, provided by Unreal Engine.
### Description
The project is my attempt at digitalizing Panic at the Dojo. The framework of which is made thanks to a very good tutorial made by Alex Quevillon. The series is called "Turn Based Tactical Combat - Unreal Engine 4 tutorial". Obviously, as you can probably guess, I've made it so that the code presented in the tutorial works for UE5.
Link to Alex channel: https://www.youtube.com/@AlexQuevillonEn

The game is by no means finished or in a fully playable state. Treat it more as a tech-demo I'm sharing this project for public use, so that everyone can work on and expand it. Sorry for the lack of proper comments on the code or documentation.
### Important notes
I've included project settings file that normally is blacklisted by the gitignore files for Unreal Engine projects. This is because the file contains custom collision trace channels required for the game to properly run the grid interactions.

The grid, for a reason I'm not sure why. doesn't spawn correctly after the first time the game is run after opening the Unreal Engine. Then it spawns normally. This bug occurs every time the engine is closed and opened.

Because the project requires a lot of different file types, I have prefixed them as such:
BP - Blueprints.
BFL - Blueprint Function Library
BPI - Blueprint Interface
ABP - Animation Blueprint
AN - Animation
SK - Skeletal Mesh
WBP - Widgets
SM - Static Meshes
TX - Texture (Though not all files that are classified as textures should have TX in front of them.
M - Material
MI - Materiał Instance
LvL - Level
IA - Input Action
F - Structure
DT - Data Table
Enum - Enumerator
Icon - Icons
Name of a widget component. Ex: Button, Spinbox - Widget component

For creating a child blueprint out of a base class, the prefix should be connected to what the parent was. For example BP_Command is a parent class of each blueprint with the “Command_” prefix.

### The game controls
Q and E - Rotates the camera horizontally  
W, A, S, D - Changes the Camera Location  
Num 9 and Num 3 - Rotates the camera vertically  
Left and Right  Mouse Buttons - Execute commands while the cursor is hovered above the grid, when commands are active. Left mouse button is also the default button that interacts with buttons on the hud.

