# Gaze-Controled Car AirSim

The current solution I have is based on this video tutorial series: https://www.youtube.com/watch?v=VWUgkcX_KoY
I originally planned to combine the AirSim Library into the code, but somehow it counldn't work. 


### For this project, you will need
- Unreal Engine
- AirSim
- Python
- CMake
- Homebrew
- pynput
- OpenCV

First of all, install everything if you haven't yet. You can find the ways to install them online. The biggest challenge I was facing was actually installing AirSim. I am a Mac user with macOS 10.14.5, and the Terminal always throw back a extra-extra-long error, and there is no solution for that. If you don't have this error, you will get a better result than what I have right now ;-)

As you can see from the code, it has the ability to detect the eyes themselves, as well as blinking. What's more, OpenCV library has the ability to detect the whole face, so you can always modify the code to enable different funtions, like smile for accelerate etc. But for what I am doing right now, I am using the eyes for direction.

The theory for behind my code is to simulate keyboard action, which are the left arrow key and the right arrow key. 

### Two Major Problems I Found

The refresh rate is technically determined by either the quality of the camera or the graphics card, or maybe both. What I have right now is a laptop with built-in webcam and integrated graphics card, so it works, but is not very responsive.

Also, the lighting and/or the camera's ISO rate would strongly affect how the program recognizes face and eyes. Whenever the lighting condition is insufficient, the detection would be inaccurate. 

I hereby grant Prof. Zichen "Frank" Xu of Nanchang University and his team to use and/or contribute to this project by any means. 



