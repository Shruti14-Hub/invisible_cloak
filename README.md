<h1 align="center">🧙‍♂️ Invisible Cloak using OpenCV</h1>

<p align="center">
  A real-time computer vision project that creates the iconic “Invisibility Cloak” effect from Harry Potter using OpenCV and color segmentation.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.7+-blue">
  <img src="https://img.shields.io/badge/OpenCV-Computer Vision-green">
  <img src="https://img.shields.io/badge/Status-Active-brightgreen">
</p>

---

## 📌 Overview

The **Invisible Cloak** project uses background subtraction and color masking to make a specific cloak (usually red) appear *transparent*, revealing the background behind it.  
It is a fun and engaging project for beginners exploring **OpenCV**, **image masking**, and **real-time video processing**.

---

## 🎥 Demo (Preview)

> *Add an output GIF or screenshots here for best showcase.*

---

## 🚀 Features

- Real-time invisibility effect  
- Smooth cloak detection using HSV color space  
- Stable background capture  
- Beginner-friendly and easy to modify  
- Supports custom cloak colors  
- Clean & optimised OpenCV pipeline  

---

## 🧠 How It Works (Core Logic)

### 1️⃣ **Background Capture**
When the script starts, the camera records a few seconds of empty background.

### 2️⃣ **Convert Frame to HSV**
HSV gives better color detection than RGB.

### 3️⃣ **Color Masking**
A specific color range (e.g., red) is isolated using:

```python
lower_red = np.array([0, 120, 50])
upper_red = np.array([10, 255, 255])
4️⃣ Replace Cloak Regions with Background

Using bitwise operations, cloak area is swapped with background pixels.

5️⃣ Final Output

Camera feed blends both layers → giving the invisibility effect.
📂 Project Structure
invisible_cloak/
│── cloak.py              # Main script
│── README.md             # Documentation
│── assets/               # (Optional) Demo images/GIFs
└── requirements.txt      # Dependencies
🎛️ Customizing Cloak Color

You can adjust HSV ranges to detect different cloak colors:
lower_color = np.array([H_min, S_min, V_min])
upper_color = np.array([H_max, S_max, V_max])
Helpful for:

Blue cloak

Green cloth

Yellow scarf

Any solid color

🛠️ Tech Used

Python 3

OpenCV (cv2)

NumPy

📈 Future Improvements

Add GUI controls for color selection

Support multi-color cloaks

Add motion stabilization

Add option to save output video

Create a web-based interface

🤝 Contribution

Contributions, issues, and feature requests are always welcome!
Feel free to open an issue and suggest improvements.

⭐ Acknowledgements

Inspired by Harry Potter’s invisibility cloak

OpenCV tutorials & community

Python Computer Vision ecosystem

<h3 align="center">⭐ If you like this project, give it a star!</h3> ```
