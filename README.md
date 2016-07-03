# ai-asissisted-scene-setup
AI assisted lightingh and shading setup on 3D software.

This is a propposal of lighting and shading assistance using artificial intelligence.

Based on Neural Style research I propose to change the direct pixel editing for parameter adjustements in lights or shading to achieve the desired style.

The parameters will be initialized using random Gaussian distribution.
The iteration, then, will follow the steps:
- Adjust the parameters
- render the scene
- check the error of the resulting picture
- repeat

If the scene should work from several angles with the same style each angle will be rendered and checked.
A proposed optimization could be to combine all pictures on one (increasing memory consumption)

If different styles are present on diferent angles of a scene some work will need to
be done to ensure that the styles dont compete when lights overlap.
