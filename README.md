# 3dViewerHTML
A 3D Viewer with Three.js and HTML5 Canvas


## Recommended tips
- Use 3d Objects with a .png render, .obj and .mtl.
- Create a loading spinner while the 3d object is loading.
- Change size of the camera dynamically.
## Target
The objective is to create a simple object viewer that can well handle low-rez 3d meshes.

## How to rotate characters and camera display
You can rotate, and zoom easily changing this values.

  ``` bash
cameraZoom: camera = new THREE.PerspectiveCamera( 50, window.innerWidth
Controls:
  controls.rotateSpeed = 1.0;
  controls.zoomSpeed = 1.2;
  controls.panSpeed = 0.2;
  controls.noZoom = true;
  controls.noPan = false;
  controls.staticMoving = false;
  controls.dynamicDampingFactor = 0.3;
  controls.minDistance = 1.1;
  controls.maxDistance = 40;
```
  
  
## How to change characters 
This viewer is easy to handle, give the path to the obj & mtl files, the ID where you want the viewer to be in, eventually a format if it can't be guessed
``` html 
<script type="text/javascript">
meshviewer({
  'objFile' : 'examples/characters/example.obj',
  'mtlFile' : 'examples/characters/example.mtl', 
  'container':'#viewer', 
  'format':'obj'});
</script>
<body> 
  <div id="viewer">
</body>
```

## Credits
Thanks to Three.JS and ideesculture
