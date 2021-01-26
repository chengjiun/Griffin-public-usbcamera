# Griffin-public

Using a pose estimation model, an object detection model built using Amazon SageMaker JumpStart, a gesture recognition system and a 3D game engine written in OpenGL running on an NVIDIA Jetson AGX Xavier, I built Griffin, a game that let my toddler use his body to fly as an eagle in a fantasy 3D world.

Watch demo video here
https://www.youtube.com/watch?v=BSbp2cRqIsc&t=6s

Read the full blog here
https://towardsdatascience.com/making-my-toddlers-dream-of-flying-come-true-with-ai-tech-82881eac01b8


# installation

## Game Engine

- see https://github.com/amhndu/fly
- install libsfml & GLEW 
    ```
    sudo apt-get install libsfml-dev libglew-dev
    ```
- comple 
    ```
    cd Game\ Engine
    mkdir build & cd build 
    cmake ..
    cd ../ & make -j4

    ```
- run api  (listening to port 2300) 
    ```
    ~/Workspace/Griffin-public/Game\ Engine/Fly
    ```

## python api

- requirements: opencv2, trt, pytorch, torch2trt, trt_pose 
- also see https://github.com/NVIDIA-AI-IOT/trt_pose
- install trt_pose
```
git clone https://github.com/NVIDIA-AI-IOT/trt_pose
cd trt_pose
sudo python3 setup.py install
cd ~/
``` 
  
