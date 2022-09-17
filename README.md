# 3D-renderer

This program takes in an .obj file as a command line argument, and then renders the 3D image on screen by
calculating lighting/color of each pixel.

Two light sources are hardcoded into the program (a main light and then a side light for more depth)

If the submitted obj is defined by triangle faces (as with the sample files included here), then a texture is also created on 
each face by playing with the normal vectors, as opposed to being rendered as though smooth)

To improve on performance, this code does not use the standard method of Ray Tracing
Instead, each pixel on of the 2D viewing screen looks to see which face of the obj contains that pixel and is closest to the camera (the screen)
Then, the pixel is rendered using that face's information from the obj file and the locations of the light sources.

Compile:

Run:

Example objs included: 
