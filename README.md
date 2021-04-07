# Half-Lambert-Unity2020LTS
  Half lambert lighting model using Unity 2020LTS with URP optimized for mobile.
# Introduction: 
 "Half Lambert" lighting is a technique first developed in the original Half-Life. It is designed to prevent the rear of an object losing its shape and looking too flat.
  To soften the diffuse contribution from local lights, the dot product from the Lambertian model is scaled by ½, add ½ and squared. The result is that this dot product, which normally lies in the range of -1 to +1, is instead in the range of 0 to 1 and has a more pleasing falloff, thus our values would be like this:
  ![chart_HL](https://github.com/nadir500/Half-Lambert-Unity2020LTS/blob/main/5084_01_09.jpg)
  
  Half Lambert is a completely non-physical technique and gives a purely percieved visual enhancement and is an example of a forgiving lighting model, reaching the result the same as in the following figure:
  ![alyx](https://github.com/nadir500/Half-Lambert-Unity2020LTS/blob/main/Alyx_lambert_half_lambert.jpg)
  
# Results in Unity: 
 ![patrick](https://github.com/nadir500/Half-Lambert-Unity2020LTS/blob/main/Recordings/gif_animation_001.gif) 
 
# TODO:
 - Add bake HL lighting model for static objects. 
 - Add additional lights interaction(baked/real-time).
 - Add more rendering stages for constant ambient, ambient cube as the following:
 ![acm paper](https://github.com/nadir500/Half-Lambert-Unity2020LTS/blob/main/8-Figure8-1.png)
 
 SIGGRAPH06 article [Shading in valve's source engine](https://dl.acm.org/doi/10.1145/1185657.1185832) is the main inspiration for the project to reach the final results and deploy the lighting model for different cartoonish styles in different lighting conditions.
# Related Links: 
 - 3D model by ChicaKnowsFNAF [Link](https://sketchfab.com/3d-models/patrick-6cfaaf749ccf4fd9a6521a79e2a2349c)
 - SIGGRAPH06 article [Link](https://dl.acm.org/doi/10.1145/1185657.1185832)
