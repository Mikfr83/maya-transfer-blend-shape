# rjRetargetBlendshape
Retarget your blendshapes between meshes with the same topology.

<p align="center"><img src="https://github.com/robertjoosten/rjRetargetBlendshape/blob/master/README.png"></p>
<a href="https://vimeo.com/170360738" target="_blank"><p align="center">Click for video</p></a>

## Installation
Copy the **rjRetargetBlendshape** folder to your Maya scripts directory:
> C:\Users\<USER>\Documents\maya\scripts

## Usage
Command line:
```python
import rjRetargetBlendshape
rjRetargetBlendshape.convert(
  source,
  blendshape,
  target,
  scale=True, 
  rotate=True, 
  smooth=0, 
  smoothIterations=0,
  space=OpenMaya.MSpace.kObject,
)
```

Display UI:
```python
import rjRetargetBlendshape.ui
rjRetargetBlendshape.ui.show()
```

## Note
Retarget your blendshapes between meshes with the same topology. There are a few options that can be helpful to achieve the desired results. 

* Scaling your delta depending on the size difference between the source and the target vertex. 
* Rotating the delta depending on the normal difference between the source and the target vertex. 
* Smoothing based on the vertex size between the retarget mesh and the blendshape mesh.
