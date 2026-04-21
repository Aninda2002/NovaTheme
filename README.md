# 🌌 NovaTheme – Gradio Theme Builder

NovaTheme is a fully customizable **Gradio theme system and visual builder** that allows you to design, preview, and export UI themes interactively. It extends Gradio’s built-in theming with enhanced styling, gradients, dark mode support, and a live preview environment.

---


## 🚀 Features

* 🎨 **Custom Theme Engine**

  * Built on top of `gradio.themes.Soft`
  * Fully configurable colors, spacing, fonts, and UI variables

* 🌗 **Dark + Light Mode Support**

  * Carefully tuned palettes for both modes
  * Smooth gradients and modern UI styling

* 🧩 **Interactive Theme Builder UI**

  * Modify theme variables in real-time
  * Instant preview of changes

* 🧠 **Smart Variable System**

  * Uses Gradio’s theme variable architecture (`primary_500`, etc.)
  * Auto-suggestions for easier customization

* 📦 **Export Ready Code**

  * Generate production-ready Python theme code

* ☁️ **Hugging Face Hub Integration**

  * Upload and share your themes easily

---

## 🏗️ Project Structure

```
├── theme.py              # NovaTheme definition
├── app.py                # Theme builder UI (Gradio app)
├── README.md             # Project documentation
```

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/novatheme.git
cd novatheme
pip install gradio gradio_client
```

---

## ▶️ Usage

Run the theme builder:

```bash
python app.py
```

This will launch a local Gradio interface where you can:

* Select a base theme
* Customize colors, fonts, spacing
* Preview changes live
* Export or upload your theme

---

## 🎨 NovaTheme Overview

NovaTheme is a custom theme class:

```python
class NovaTheme(Soft):
    ...
```

### Key Customizations:

* 🌈 Gradient buttons (`primary` / `secondary`)
* ⚡ Minimal shadows for modern UI
* 🎯 Improved contrast and accessibility
* 🔤 Google Fonts integration (`Quicksand`, `IBM Plex Mono`)

---

## 🧪 Example Usage

```python
import gradio as gr
from theme import NovaTheme

with gr.Blocks(theme=NovaTheme()) as demo:
    gr.Markdown("# Hello NovaTheme ✨")

demo.launch()
```

---

## 🛠️ Customization Guide

### 1. Core Variables

* `primary_hue`
* `secondary_hue`
* `neutral_hue`
* `text_size`, `spacing_size`, `radius_size`

### 2. Theme Variables

Use Gradio variable syntax:

```
*primary_500
*neutral_900
*spacing_md
```

### 3. Fonts

Supports:

* Local fonts
* Google Fonts (auto-loaded)

---

## ☁️ Upload to Hugging Face Hub

Inside the UI:

1. Enter theme name
2. Add your HF token
3. Click **Upload**

Then use it like:

```python
gr.Blocks(theme="username/theme-name")
```

---

## 📸 Preview Components

The demo app includes:

* Buttons, sliders, dropdowns
* Chatbot UI
* Tables, JSON, file upload
* Media (image, video, gallery)

This ensures your theme works across all Gradio components.

---

## 🧠 How It Works

* Uses `gr.themes.Base.set()` to override variables
* Dynamically generates CSS
* Injects styles into DOM in real-time
* Tracks history for undo functionality

---

## 🔄 Undo & Live Rendering

* Every change is tracked
* Undo button restores previous state
* Instant re-render using event listeners

---

## 📌 Requirements

* Python 3.9+
* Gradio 4.x+

---

## 🤝 Contributing

Pull requests are welcome!
If you’d like to improve NovaTheme:

* Add new presets
* Improve UI
* Optimize performance

---

## 📄 License

MIT License

---

## ⭐ Support

If you like this project:

* ⭐ Star the repo
* 🍴 Fork it
* 🧠 Share your themes

---

## 🔥 Future Improvements

* Theme presets library
* Export as JSON/CSS
* Theme comparison mode
* Plugin system

---

## 👨‍💻 Author

Built for advanced UI customization using Gradio.

---

**NovaTheme = Clean UI + Full Control 🚀**
