# Simple Side By Side Picture Viewer (SBS)

This is a simple web-based application (HTML/CSS/JavaScript) designed to display Side-by-Side (SBS) stereoscopic images using the alternating/stroboscopic viewing method, ideal for certain 3D displays or for experimenting with stereo vision.

## Features

* **Image Loading:** Drag-and-drop or select any PNG or JPG image file.
* **Alternating View:** Displays the Left and Right halves of the SBS image in rapid succession. The image scales automatically to fit entirely within the browser window.
* **Adjustable Speed:** Control the alternation frequency (10ms to 1000ms).
* **Parallax Adjustment:** Fine-tune the horizontal offset (in pixels) of the Right view to set the "zero depth plane" and eliminate translation artifacts. Adjust settings using on-screen sliders, mouse wheel, and keyboard arrows.

## What is a Side-by-Side (SBS) Image?

A Side-by-Side (SBS) image is a format for **stereoscopic 3D content**. It consists of two separate images—one intended for the left eye and one for the right eye—placed horizontally adjacent to each other within a single file.

The primary use of the SBS format is to convey both views in one stream, which is then processed by a 3D display (like a 3D TV or VR headset) to separate and present each image to its respective eye, creating the illusion of depth.

## How to Use

The script is a single-page application and does not require a web server; you can run it directly from your file system.

1.  **Download:** Clone this repository or download the `index.html` and `script.js` files.
2.  **Open:** Open the `index.html` file in any modern web browser (Chrome, Firefox, Edge, etc.).
3.  **Load Image:**
    * **Drag & Drop:** Drag a Side-by-Side image file (e.g., `image.jpg`) onto the designated area or directly onto the viewer once an image is loaded.
    * **Select File:** Click the "click to select" link to open a file selection dialog.
4.  **Adjust Controls:**
    * **Speed (Up/Down Arrows):** Use the slider or the **Up** and **Down** arrow keys to set the duration (in milliseconds) for which each view is displayed.
    * **Parallax (Left/Right Arrows or Mouse Wheel):** Use the slider, the **Left** and **Right** arrow keys, or the **Mouse Wheel** over the viewer to shift the Right image horizontally. Adjust this until the image appears correctly aligned at the depth level you desire.

## How to Get SBS Images

SBS images can be created through several methods:

1.  **Stereo Camera Systems:**
    * **Dedicated 3D Cameras:** Cameras designed with two lenses, spaced roughly at the average human interocular distance (about 6.5 cm).
    * **Dual-Camera Rigs:** Two separate cameras mounted together (e.g., two smartphones or DSLRs).

2.  **Computer-Generated Imagery (CGI):**
    * 3D rendering software (like Blender, Maya, or Three.js) can easily render a scene from two virtual cameras with a slight horizontal offset.

3.  **AI and Depth Mapping:**
    * Advanced image processing, often using Deep Learning (AI), can take a standard 2D image and calculate a **Depth Map** (a grayscale image where lighter areas are closer and darker areas are farther).
    * This depth information is then used to **synthesize** a second, offset image (the "right eye" view) from the original (the "left eye" view), resulting in a convincing 3D SBS image.

