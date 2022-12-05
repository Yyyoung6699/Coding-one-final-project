# Coding-one-final-project
Coding one final project of Luyang Xing
Vedio link: https://youtu.be/vKFPkon1JlM
Mimic link: https://mimicproject.com/code/2fc0db25-2cfc-4a8e-8213-c50aad992308

Project Description
In the coding one course I learned about sound, 2D and 3D code. I tried to make my week3 2D homework in 3D and adding sound visualization elements. My code is not complicated, but I spent a lot of time getting the visual effects to fit the sound. When running it, the vibrating spheres and color changes with the powerful drums are like a colorful speaker, giving a visual and auditory impact.

Sound
Firstly, I used coding of week2 to add two audio samples via maximilian.js and used maxiClock to set the conditions for the audio to play. I tried to learn the extra tutorial provided by my tutor on the FFT analyser and use it to get the aspectrogram of sounds, but it didn't work. I was left with the option of a BPM counter for sound visualisation.

Scene and BPM counter
As with all projects I use three.js to add a scene, camera and a PointLight with random colours. in addition I add a sphere at the origin (0,0,0) and make its colour randomly red or yellow and the scale randomly changes within a certain range to match the beats of the music. Interestingly, when I was trying to add a normal pan animation to the camera, I thought of using the BPM counter to control the camera position randomly if(myClock.playHead%8===4){}, and after a lot of practice I found that it worked great and was full of rhythm. It is fantastic. However, when I tried to use this method to control the colour and scale, it didn't work.

Loop and animation
I created several small balls to enrich the image, using for loop in conjunction with the Cartesian functions learnt in the week3 and week6 course to create groups of looping balls that rotate around the origin. In my week3 homework the rotation effect was controlled by the mouse position, but I didn't think it was suitable for this work, so I changed it to automatic animation. Here I ran into a problem, the balls after the for loop can not set the rotation animation in function draw(). After searching some cases I tried to solve this by setting the balls to separate arrays var array = []; array[i] =new THREE.Mesh(geometry,material); and then adding animation to the array. I tried a lot of different materials. I didn't add a map to the balls because I thought a solid colour would be more appropriate for this form of interaction.

Future
In the future, I will consider building on this work. In addition to some particle visual effects, I hope to add an FFT analyser to relate the movement of the balls to pitch and timbre, so that users can upload different music and observe the different visual changes, enabling more sound visualisation.
