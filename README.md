# Interactive fluid dynamics

**Hardcoded preset - whirlpool formation in a hourglass**

This is binary demo (without source code) sandbox for fluid dynamics.  
Based on heavily interfaced and updated sources https://github.com/wme7/openLBMflow.

Made with c++, DirectX, Qt UI, OpenMP optimizations

Sources have too raw quality yet to be published, but may provide them on request.

On the next images:  
- Two fluids are simulated, in this setup they bechave close to low dense bubble (~air) in liquid.
- Red lines are dynamically calculated streamlines, i.e. if an external particle appears in the fluid, it will travel along these lines.  
Color of streamlines varies slightly from black to red because it directly relates to velocity (reddier = faster).  
Streamlines can intersect border between fluids because of simplified calculations.


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
