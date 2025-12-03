# Halftone Generator

> **Transform your images and videos into retro, dot-matrix style halftone art in real-time.**

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)

**Halftone Generator** is a high-performance, browser-based visual engine. It allows users to upload images or videos and instantly render them as dynamic halftone patterns. Built with raw HTML5 Canvas and Vanilla JavaScript, it performs complex pixel manipulation and dithering algorithms entirely on the client side.

---

## 📸 Screenshots

*(Add screenshots of your application here)*

---

## ✨ Key Features

* **⚡ Real-Time Processing:** Instantly renders changes as you tweak sliders, utilizing the HTML5 Canvas API for high-performance pixel manipulation.
* **🎥 Video Support:** Not just for static images—upload video files (`.mp4`, `.webm`) and watch them play as dynamic halftone animations.
* **🎛️ Advanced Controls:**
    * **Grid Size:** Control the density and size of the halftone dots.
    * **Image Correction:** Adjust Brightness, Contrast, and Gamma to perfect the input before processing.
    * **Smoothing:** Built-in box blur to reduce noise before halftoning.
* **🎨 Dithering Algorithms:**
    * **Floyd-Steinberg:** Error diffusion for smooth gradients.
    * **Ordered:** Structured, Bayer-matrix style patterning.
    * **Noise:** Adds organic texture and grain.
* **💾 Export:** Download your high-resolution creations as PNG files or webm files.
* **🔒 Privacy First:** All processing happens locally in your browser. No files are uploaded to any server.

---

## 🛠️ Technologies Used

* **Core:** HTML5, CSS3 (Variables + Flexbox)
* **Logic:** Vanilla JavaScript (ES6+)
* **Rendering:** HTML5 Canvas API (`getImageData`, `putImageData`)
* **Performance:** `requestAnimationFrame` for efficient video rendering loop

---

## 🚀 Getting Started

Since this is a client-side web application, you don't need to install any heavy dependencies.

### Prerequisites

* A modern web browser (Chrome, Firefox, Safari, Edge).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/imvarun18/Halftone-Generator.git](https://github.com/imvarun18/Halftone-Generator.git)
    ```
    *(Note: Replace URL with your actual repo link)*

2.  **Navigate to the project directory:**
    ```bash
    cd Halftone-Generator
    ```

3.  **Run the App:**
    * Simply open `index.html` in your browser.

> **Tip:** For the best experience with video loading, it is recommended to use a live server (e.g., VS Code "Live Server" extension) to avoid local CORS restrictions, though file uploads will work fine directly.

---

## 🎮 Usage Guide

1.  **Upload Media:** Click the upload area or drag and drop an image or video file.
2.  **Adjust Grid:** Use the **"Grid Size"** slider to determine how "retro" the image looks. Larger grid = bigger dots = more abstract.
3.  **Tune Visuals:**
    * Use **Contrast** to make the dots pop.
    * Use **Gamma** to adjust the mid-tones.
    * Use **Smoothing** if your source image is too noisy.
4.  **Select Algorithm:** Choose a dithering type from the dropdown to change how the shading is calculated.
5.  **Export:** Click **"Export PNG" or "Export Video"** to save your work.

---

## 🧮 Algorithms Explained

This project implements several pixel-processing techniques from scratch:

* **Halftone Generation:** The image is divided into a grid. The average grayscale value of pixels within each grid cell determines the radius of the circle drawn in that cell.
* **Floyd-Steinberg Dithering:** A technique that diffuses the quantization error of a pixel to its neighboring pixels. This creates a much smoother visual result for gradients compared to standard thresholding.
* **Ordered Dithering:** Uses a fixed "Bayer Matrix" to threshold pixels, resulting in a cross-hatch style look often seen in early computer graphics.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1.  Fork the project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

<div align="center">
  <sub>Built with ❤️ by Varunsai</sub>
</div>
