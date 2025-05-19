# Web-based AR 3D Model Viewer

This is a simple web-based AR application that displays 3D models using image markers. It uses AR.js and A-Frame for the AR functionality.

## Prerequisites

- A modern web browser (Chrome, Firefox, or Safari recommended)
- A webcam
- The Hiro marker image (you can find it [here](https://raw.githubusercontent.com/AR-js-org/AR.js/master/data/images/HIRO.jpg))

## How to Use

1. Open the `index.html` file in your web browser
2. Click the "Start AR" button to grant camera permissions
3. Print or display the Hiro marker image on another device
4. Point your camera at the Hiro marker
5. You should see a yellow cube appear on top of the marker

## Customizing the 3D Model

To change the 3D model, modify the content inside the `<a-marker>` tag in `index.html`. You can:

- Use different A-Frame primitives (box, sphere, cylinder, etc.)
- Load custom 3D models using the `<a-entity>` tag with a gltf-model
- Adjust the position, rotation, and scale of the model

## Example of loading a custom 3D model:

```html
<a-marker preset="hiro">
    <a-entity
        position="0 0.5 0"
        rotation="0 0 0"
        scale="1 1 1"
        gltf-model="path/to/your/model.gltf">
    </a-entity>
</a-marker>
```

## Notes

- Make sure you have good lighting conditions for better marker detection
- Keep the marker steady and visible to the camera
- The marker should be printed or displayed on a flat surface 