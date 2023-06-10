# Ex-03-Game-Programming-

# AIM:
To Change the third person character mesh using animations.

# PROCEDURE:
1.Import the animation assets: Obtain the animation files for jump, walk, and idle in a compatible format such as FBX or BVH. To import the animations, go to the Content Browser panel in Unreal Engine, right-click in the desired folder, and select Import

2.Create a Separate folder and Import the Animations to avoid any chaos

3.Create an animation blueprint: In Unreal Engine, animation blueprints are used to control character animations. To create a new animation blueprint, follow these steps: a. Right-click in the folder where you imported the mesh and select Create > Animation > Animation Blueprint.

a. In the Animation Blueprint Editor, click on the Event Graph tab.

b. Drag the new character mesh from the Content Browser and drop it onto the graph.

c. Connect the Output Pose pin of the mesh node to the Final Animation Pose pin of the Final Animation Pose node.

d. Save the animation blueprint.

4.Open the animation blueprint: Open the animation blueprint you created for your character in the Animation Blueprint Editor.

5.Create animation slots: Animation slots help organize different animations and control their blending. To create animation slots, follow these steps: a. In the AnimGraph tab of the Animation Blueprint Editor, right-click in the graph and select Add State Machine > Animation Layer.

a. Double-click the newly created animation layer to open it.

b. Right-click in the graph of the animation layer and select Add State Machine. d. Double-click the newly created state machine to open it.

c. Right-click in the graph of the state machine and select Add State.

e. Rename the state to "Jump" and repeat steps e and f to create states for "Walk" and "Idle".

6.Add animation assets to states: In each state, you will assign the corresponding animation assets. To add animation assets to the states, follow these steps: a. Double-click the "Jump" state to open it.

a. Right-click in the graph and select Add State Result.

b. Drag and drop the jump animation asset onto the graph.

c. Connect the Result node to the jump animation asset.

d. Repeat steps a to d for the "Walk" and "Idle" states, assigning the appropriate animation assets.

7.Create required Variables for the state’s like “ISJUMP”, “SPEED”.

8.Set up transition rules: Transition rules determine when the character transitions between different animations. To set up transition rules, follow these steps: a. Double-click the "Jump" state to open it.

a. Right-click in the graph and select Add Transition Rule.

b. Drag the transition rule from the "Jump" state to the "Idle" state.

c. Repeat steps a to c for the "Walk" state, creating transitions from "Idle" to "Walk" and from "Walk" to "Idle".

d. Configure the transition rules based on your desired conditions. For example, you might want to trigger the transition from "Idle" to "Jump" when the character jumps, and from "Jump" to "Idle" when the jump animation is finished.

9.Create a Anim Montage in Animation Folder To Manage the montages of the animations.

10.Connect the animation blueprint to the character blueprint: To connect the animation blueprint to the character blueprint and enable the animations in the game, follow these steps: a. Open the character blueprint associated with the third person character.

a. In the Viewport tab of the Blueprint Editor, select the mesh component of the character.

b. In the Details panel, under the Animation category, find the Animation Blueprint property.

c. Click on the dropdown menu and select the animation blueprint you created.

11.Test the character: Compile and save all the changes in the blueprints and animations. Now, you can test the character's jump, walk, and idle animations by clicking the Play button in the Unreal Editor.

# OUTPUT:

# Stem machine :
![1](Screenshot%202023-06-10%20191910.png)

# state Diagram :

![2](Screenshot%202023-06-10%20191939.png)

# Variables :

![3](Screenshot%202023-06-10%20192001.png)

# Idle to Walk :

![4](Screenshot%202023-06-10%20192019.png)

# Walk to idle :

![5](Screenshot%202023-06-10%20192052.png)

# Walk to jump :

![6](Screenshot%202023-06-10%20192110.png)

# Jump to walk :

![7](Screenshot%202023-06-10%20192129.png)

# Jump to idle :

![8](Screenshot%202023-06-10%20192151.png)



# Animation Blueprint :

![9](Screenshot%202023-06-10%20192210.png)



![10](Screenshot%202023-06-10%20192241.png)

# Third person Blueprint :

![11](Screenshot%202023-06-10%20192302.png)






# RESULT:
The third person character mesh has been successfully changed using animations.