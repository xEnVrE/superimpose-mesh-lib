# %Superimpose an object {#tutorial_superimpose}

This tutorial introduces the basic steps to superimpose an object, i.e. a mesh,
on top of an image by using the [SICAD](@ref SICAD) helper class and its methods.<br>

Just have a look at the following commented ready-to-go snippet code!.<br>

\includelineno tutorial_code/tutorial_superimpose.cpp

Here are the shaders and the Space Invaders mesh model:
 - [Model vertex shader](https://github.com/robotology/superimpose-mesh-lib/blob/gh-pages/doxygen/tutorial_code/shader_model.vert "Model vertex shader")
 - [Model fragment shader](https://github.com/robotology/superimpose-mesh-lib/blob/gh-pages/doxygen/tutorial_code/shader_model.frag "Model fragment shader")
 - [Background vertex shader](https://github.com/robotology/superimpose-mesh-lib/blob/gh-pages/doxygen/tutorial_code/shader_background.vert "Background vertex shader")
 - [Background fragment shader](https://github.com/robotology/superimpose-mesh-lib/blob/gh-pages/doxygen/tutorial_code/shader_background.frag "Background fragment shader")
 - [Space Invader fiend](https://github.com/robotology/superimpose-mesh-lib/blob/gh-pages/doxygen/tutorial_code/Space_Invader.obj "Space Invader fiend")

⚠️ The four shaders must have that exact names, i.e.:
 - _shader_model.vert_ for the model vertex shader
 - _shader_model.frag_ for the model fragment shader
 - _shader_background.vert_ for the background vertex shader
 - _shader_background.frag_ for the background fragment shader

You should get something like this:
![👾](alien.jpg)

You can now proceed to the next tutorial: [how to add a background](@ref tutorial_superimpose_background)!
