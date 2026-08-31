# Easy Blob Track for TouchDesigner

**Easy Blob Track** is a plug-and-play TouchDesigner component (`.tox`) designed to simplify real-time blob detection. It handles the heavy lifting of video analysis and exposes ready-to-use visual layers and data streams out of the box—no complex setup required.

Whether you are building interactive installations, tracking stage performers, or driving visual effects with motion, **Easy Blob Track** gets you up and running in seconds.

### 🔓 Open & Collaborative

This tool was created for the TouchDesigner community. Feel free to **use it in your projects, remix the internal network, fix bugs, or improve its features**. If you make an awesome upgrade, pull requests and contributions are always welcome!

Voici la section **Structure** complète au format Markdown, combinant l'intro explicative et la documentation des entrées/sorties :

### Inputs

* **`TOP Input 1`** *(Top purple connector)*: The raw video source or live camera feed to analyze.
* **`CHOP Input 1`** *(Bottom blue connector)*: Optional control signal for dynamic parameter overrides (e.g., threshold automation, tracking reset).

### Outputs

| TOP Output | Connector Name | Description & Use Case |
| :--- | :--- | :--- |
| **Output 1** | `dot` | **Center Points**: Generates points at the centroid of each detected blob. |
| **Output 2** | `edge` | **Outlines**: Renders the outer contours of detected blobs. |
| **Output 3** | `mask` | **B&W Mask**: Binary matte (white = blob, black = background). Used for keying, clipping, or applying targeted shaders. |
| **Output 4** | `data` | **Data Texture (TOP-as-Data)**: Displays the blob ID as an overlay on the image (e.g., 1434). |
| **Output 5** | `video` | **Video Feed / Pass-through**: Passes the original or pre-processed video stream through for live visual monitoring and overlay alignment. |
