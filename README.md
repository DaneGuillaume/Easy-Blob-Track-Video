# Easy Blob Track for TouchDesigner

**Easy Blob Track** is a plug-and-play TouchDesigner component (`.tox`) designed to simplify real-time blob detection. It handles the heavy lifting of video analysis and exposes ready-to-use visual layers and data streams out of the box—no complex setup required.
Whether you are building interactive installations, tracking stage performers, or driving visual effects with motion, **Easy Blob Track** gets you up and running in seconds.

## 🔓 Open & Collaborative

This tool was created for the TouchDesigner community. Feel free to **use it in your projects, remix the internal network, fix bugs, or improve its features**. If you make an awesome upgrade, pull requests and contributions are always welcome!
Voici la section **Structure** complète au format Markdown, combinant l'intro explicative et la documentation des entrées/sorties :

## 📐 .tox Structure

### Inputs

| Input Connector | Connector Name | Description |
| :--- | :--- | :--- |
| **Input 1** | `video` | Raw video source or live camera feed to analyze. |
| **Input 2** | `background` | Background input directly from the Blob Track TOP (used for background subtraction). |

### Outputs

<img width="3610" height="1279" alt="layer" src="https://github.com/user-attachments/assets/318f1da3-4325-47bc-914c-c1688efbb9cc" />

| TOP Output | Connector Name | Description & Use Case |
| :--- | :--- | :--- |
| **Output 1** | `dot` | **Center Points**: Generates points at the centroid of each detected blob. |
| **Output 2** | `edge` | **Outlines**: Renders the outer contours of detected blobs. |
| **Output 3** | `mask` | **B&W Mask**: Binary matte (white = blob, black = background). Used for keying, clipping, or applying targeted shaders. |
| **Output 4** | `data` | **Data Texture (TOP-as-Data)**: Displays the blob ID as an overlay on the image (e.g., 1434). |
| **Output 5** | `video` | **Video Feed / Pass-through**: Passes the original or pre-processed video stream through for live visual monitoring and overlay alignment. |

### 📸 Showcase & Community Projects

* 🎬 [Easy Blob Track Project #1 on Instagram](https://www.instagram.com/p/Dclj_XzsScp/)
* 🎬 [Easy Blob Track Project #2 on Instagram](https://www.instagram.com/p/DcoS2MEshtB/)

### 👏 Credits & Acknowledgments

* **Developer**: Created by [Dane_909](https://github.com/DaneGuillaume)
* **TouchDesigner Version**: Developed and tested on **TouchDesigner 2025.33070**
* **Special Thanks**: A big thank you to [Dean Cheesman](https://www.youtube.com/@DeanCheesman) for his incredible tutorials and resources on TouchDesigner, which greatly inspired and helped shape this component.
