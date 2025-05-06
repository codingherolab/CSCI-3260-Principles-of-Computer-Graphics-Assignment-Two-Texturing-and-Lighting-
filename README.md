# CSCI-3260-Principles-of-Computer-Graphics-Assignment-Two-Texturing-and-Lighting-

Download Here: [CSCI 3260 Principles of Computer Graphics Assignment Two: Texturing and Lighting](https://codingherolab.com/product/csci-3260-principles-of-computer-graphics-assignment-two-texturing-and-lighting/)

For Custom/Original Work email codingprolab@gmail.com/whatsapp +1(541)423-7793

I. Introduction
In this assignment, you are required to build an even more realistic and complex scene with OpenGL. To
achieve this task, you will experience more features in OpenGL, including lighting, complex model building and
loading, texture mapping and interactive events. You are about to use primitive drawing or load a 3D model from
an .obj file directly and then view/model the transformation to create this 3D scene. Texture mapping and lighting
will be employed to make the scene and objects more realistic. Mouse/keyboard inputs and window event
handling will help realizing the interactive animation.
Fig. 1: The scene drawn by the demo program.
In this assignment, there are two models in the scene. One (the ground plane) is relatively simple, the other
(jeep) is complex. We can design the vertex attributes of the ground plane by ourselves. However, for the jeep, it
is so complicated that we need to load the model by .obj file. In addition, the ground plane and the jeep are
rendered with different textures with lighting effect. The scene we watch can be controlled by the user inputs. You
can use the scene you modeled in assignment 1 to enrich the scene.
II. Implementation Details
Task 1: Loading complex object
Use the Open Asset Import Library, or the function ‘bool loadOBJ()’ which we have given to load at least
one complex model. In this part, you can use bool loadOBJ() function by modifying the ‘void
sendDataToOpenGL()’ subroutines.
We have provided the models in the demo program, i.e. plane.obj and jeep.obj. You are encouraged to
download other .obj file from Internet or use Blender to design your own object.
Task 2: Texture Mapping & Lighting
You need to map different textures to the two models, i.e. the ground plane and the jeep in the demo program.
You first need to create one OpenGL texture and set the texture parameter by modifying the ‘GLuint
loadBMP_custom(const char * imagepath)’ subroutines. Then, load and bind textures to different models in
‘void sendDataToOpenGL()’ and ‘void paintGL(void)’ subroutines, respectively.
Here, we have also provided the textures of models in the demo program, i.e. plane_texture.bmp and
jeep_texture.bmp. You are also encouraged to download other textures from Internet.
In addition, the 3D scene should be illuminated with at least two light sources. One should be an environment
light. For the other light source, you can decide the position and color of that by yourself. The main purpose of
this light source is to produce the diffuse light and specular light effect on the models. You can do this by
modifying the ‘void paintGL(void)’ subroutines.
Task 3: Interactive Events and Animation
In this task, you are required to implement the following interactive events and animation:
(a) Lighting control
Press key “q” and key “w” to increase and reduce brightness of diffuse light, respectively.
Press key “z” and key “x” to increase and reduce brightness of specular light, respectively.
(b) View control
Control the position of camera by mouse, which means:
When mouse moves up, the whole scene you see moves down.
When mouse moves left, the whole scene you see moves right.
(c) Model animation and control
The complex model on the ground plane can rotate about the z-axis and we can use key ‘s’ to control that
whether stop or continue the rotation.

In this task, you may modify the following subroutines:
void keyboard(unsigned char key, int x, int y) ;
void PassiveMouse(int x, int y);
Bonus Task: Enhance the visual effect of your scene (maximum 20%)
OpenGL provides many functions for your program to create various visual effects. You can study them by
yourself and introduce them into the assignment. Here are some suggested improvements:
• Loading more than one complex model and map other textures onto them to form a meaningful scene, for
example, car park. (10%)
• Press arrow keys “↑↓←→” to control the movements of the complex model above the ground plane.
(10%)
• Shadow mapping (10%)
• Any other interesting effects
III. Grading Scheme
Your assignment will be graded by the following marking scheme:
Basic (80%)
Loading the complex model 10%
Texture mapping 20%
Lighting of environment light 5%
Lighting of light source you designed 15%
Lighting control 15%
View control 10%
Model animation 5%
Bonus 20%
Total: 100%
Note: no grade will be given if the program is incomplete or fails compilation.
IV. Guidelines to submit programming assignments
1) You are suggested to write your programs on Windows, since there will be enough technical support. If you
developed the program in other platforms, make sure your program can be compiled and executed on
Windows as the program will only be tested on this platform. The official IDE is Visual Studio C++ 2015.
2) Modify the provided submit.cpp & VertexShader.glsl & FragmentShader.glsl, and provide all your code in this
file. No other additional .cpp or .h files are allowed. Type your full name and student ID in main.cpp. Missing
such essential information will lead to mark deduction (up to 10 points).
3) We only accept OpenGL code written in programmable pipeline. No points will be given if your solution is
written in fixed pipeline.
4) Zip the source code file (i.e. submit.cpp & VertexShader.glsl & FragmentShader.glsl), the executable file (i.e.,
submit.exe), and the readme file for other interactive events you designed (i.e., readme.txt) in a .zip. Name it
with your own student id (e.g. 1155012345.zip). There should be exactly five files in your submitted package.
5) Submit your assignment via eLearn Blackboard. (https://elearn.cuhk.edu.hk/)
6) Please submit your assignment before 11:59 p.m. of the due date. Late submission will be penalized by 10%
deduction per day.
7) In case of multiple submissions, only the latest one will be considered.
8) Fail the course if you copy.
