---
layout: project
type: project
image: img/
title: "Augmented Reality Tamagotchi Simulator"
date: 2024
published: true
labels:
  - Augmented Reality
  - Game Design
  - C#
  - Unity

summary: "I created an augmented reality simulator inspired by Tamagotchi games."
---
<video width="600" controls>
  <source src="../video/ar_tamagotchi_video.mp4" type="video/webm">
  Your browser does not support the video tag.
</video>

Everyone loves the handheld digital pets Tamagotchi. But what if you could expand that concept to bring your pet directly into your room?

This augmented reality (AR) game, built for the Quest 3, uses spatial awareness to integrate your current surroundings into the gameplay. Digital objects in the game environment interact seamlessly with real-world surroundings. Your Tamagotchi pet, which is a dragon in this case, has two key needs: hunger and happiness, represented by status bars that decrease over time.

To keep your dragon healthy and happy, you’ll need to feed it cake to satisfy its hunger and play fetch to keep it happy. But beware—if either bar gets too low, your pet won’t hesitate to set your room on fire with its fire breath! By neglecting your dragon for too long, it could die—so take good care of it.

## How it was created
This AR experience was developed using the Unity game engine and its AR Foundation package to scan and interact with real-world environments.

Physics and object colliders are used to detect interactions with the dragon. Game objects like the soccer ball (for fetch) and food items (like cake) are tagged to distinguish their purpose. Depending on the object, collisions with the dragon trigger different animations and sounds, bringing it to life.

One of the biggest challenges was implementing the fetch mechanic. After the player throws the soccer ball, they press the X button on the controller to command the dragon to retrieve it. The tricky part was ensuring the dragon could locate the player’s position within the room and return the ball 1-2 feet in front of them.

This was solved using AR Foundation’s ability to track the Quest 3’s camera. By assigning a “Player” tag to the camera rig, the dragon can find the player’s location and successfully return the ball. 

## Unity Assests Used
- **Dragon Model:** [View the dragon model here](https://assetstore.unity.com/packages/3d/characters/animals/mammals/tiny-dragon-161097)
- **Food Items:** [View the food items here](https://assetstore.unity.com/packages/3d/props/food/3d-props-adorable-foods-31249)
- **Soccer Ball Model:** [View the soccer ball model here](https://assetstore.unity.com/packages/3d/low-polygon-soccer-ball-84382)






