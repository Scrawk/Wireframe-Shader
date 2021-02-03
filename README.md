# Wireframe-Shader

There are times when you want to show a mesh in wireframe mode. It could be part of the look of your game or you may want to see whats going on for debugging reasons. Unity makes this quite easy by enabling wireframe mode in the editor but it would be nice if you could have a wireframe material to drag onto the mesh.

This is a shader that can be used to make a wireframe material. It uses the geometry pipeline to 'see' the triangle and calculate the fragments distance from the triangles edge. You can then use this information to add a line around the triangle. As the shader needs the geometry pipeline there are some limitations. Geometry shaders are a SM4 (dx10) feature only in Unity so you will need to have dx11 enabled.

The wireframe shader used here is based on a openGL shader posted on the [Little Grasshopper blog](http://prideout.net/blog/) and can be found in the ' Triangle tessellation in openGL 4.0' article.


![WireframeShader](./Media/Wireframe.jfif)
