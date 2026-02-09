# 🎨 UNIBEN Awards DP & Flyer Generator

A premium, browser-based graphic automation tool designed for the **UNIBEN Awards**. This application allows nominees and participants to generate high-quality, personalized nomination flyers in seconds without needing professional design software like Photoshop.

## ✨ Key Features

* **Custom Template Support:** Upload your own PNG/JPG flyer templates or use the built-in default.
* **Precision Photo Adjustment:** Real-time controls for **Zoom**, **Horizontal Positioning**, and **Vertical Positioning** to ensure your selfie fits perfectly in the frame.
* **Dynamic Text Rendering:** Automatic word-wrapping and shadow effects for names, award categories, and faculties.
* **Instant Preview:** See changes as you type; no refresh required.
* **High-Resolution Output:** Generates a  pixel image optimized for WhatsApp DPs, Instagram, and X (Twitter).
* **Client-Side Processing:** All image processing happens in the browser—your personal photos are never uploaded to a server, ensuring 100% privacy.



## 🛠️ Technical Overview

The project is built using a "Vanilla" stack for maximum performance and zero dependencies:

* **HTML5 Canvas API:** Used for complex image layering, circular clipping, and text typography.
* **CSS3 Animations:** Features `backdrop-filter` for glassmorphism and keyframe animations for a smooth UI experience.
* **JavaScript (ES6+):** Manages the state for image transformation and real-time canvas re-drawing.



## 🚀 How to Use

1. **Select Template:** Upload the official award template or click "Load Default Template."
2. **Upload Photo:** Choose a clear selfie. Once uploaded, the **Photo Controls** will appear.
3. **Adjust:** Use the sliders to zoom and position your face within the circular border.
4. **Enter Details:** Type in your Full Name, Nomination Category, and Faculty/Department.
5. **Generate & Download:** Click **Generate DP** to finalize the render, then **Download Image** to save the `.png` file to your device.



## ⚙️ Configuration (for Developers)

You can easily customize the flyer layout by modifying the `CONFIG` object in the script tag:

```javascript
const CONFIG = {
    canvasWidth: 1054,
    canvasHeight: 1280,
    userPhoto: {
        x: 527,          // Center X coordinate for the photo
        y: 645,          // Center Y coordinate for the photo
        radius: 160,     // Size of the circular crop
        borderWidth: 12, // Gold border thickness
        borderColor: '#FFD700'
    },
    text: {
        name: { y: 885, fontSize: 72 }, // Position and size for Name
        role: { y: 985, fontSize: 42 }  // Position and size for Category
    }
};

```



## 📂 Project Structure

* `index.html`: Contains the UI structure, CSS styling, and the JavaScript logic.
* `default-template.jpg` (Optional): Place a default background in the root folder to use the auto-load feature.



## 🛡️ Privacy & Security

> **Note:** This tool is a "Static Web App." It does not use a database or a backend. All image manipulations are performed locally on the user's device. No data is stored or transmitted.



## 💜 Credits

Developed by **Adisaac Tech Innovations Ltd**.
*Empowering students through digital innovation.*
