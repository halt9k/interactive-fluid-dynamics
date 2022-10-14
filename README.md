# Fluid dynamics realtime demo

**Hardcoded preset - whirlpool formation in a hourglass**

This is bianry demo (without source code) sandbox for fluid dynamics.  
Based on heavily interfaced and updated sources https://github.com/wme7/openLBMflow.

Made with c++, DirectX, Qt UI, OpenMP optimizations

Source code has too raw quality to be published, however - if will be free (not guaranteed now due to political situation) and
if will have time - there are plans to finish, polish and publish it. 
Sources are placed in my private repo and if this account became unresponsive for more than 6mon I give permision to public them.

On the next images:  
- Two fluids are presented, they can also be intuitevly thought of "blue = air", "light green = water" or similar.
- Red lines are dynamically calculated streamlines, i.e. if an external particle appears in the fluid, it will travel along these lines.  
Color of streamlines varies slightly from black to red because it directly relates to velocity (reddier = faster).  
Streamlines can intersect border between fluids not because this is correct, but because streamlines calculation was simplified.


Applying potential force to two phase fluid:
**![full process video](https://raw.githubusercontent.com/halt9k/interactive-fluid-dynamics/main/desc/Simple.mp4)**  

Preview:  
![](https://github.com/halt9k/interactive-fluid-dynamics/blob/main/desc/Simple.png?raw=true)  

Same, but with initial disturbance:
**![full process video](https://raw.githubusercontent.com/halt9k/interactive-fluid-dynamics/main/desc/Whirpool.mp4)**  

Preview:  
![](https://github.com/halt9k/interactive-fluid-dynamics/blob/main/desc/Whirpool.png?raw=true)  


Code parallelization (omp directives) test on 8 core CPU:
![](https://github.com/halt9k/interactive-fluid-dynamics/blob/main/desc/Parallelization.png?raw=true)  
