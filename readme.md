# Offline OCR Editor (v3)

A powerful, privacy-first desktop application built with Tauri and Vue 3, designed for high-performance Optical Character Recognition (OCR) and rich-text editing.

## 🚀 Features

- **Offline OCR Inference:** Run OCR models completely offline on your local machine for ultimate privacy. No internet connection required after the initial model download.
- **Math Formula Recognition:** Seamlessly convert images of mathematical formulas and equations into LaTeX code.
- **Rich-Text Editor:** A built-in, fully-featured WYSIWYG editor (powered by Tiptap) supporting markdown shortcuts, heading formatting, text styling (bold, italic, strikethrough), and lists.
- **Cross-Platform Support:** Built with Tauri, providing a lightweight desktop experience for Windows (and potentially other platforms), with shared UI logic for mobile devices.
- **Cloud Synchronization & Subscriptions:** Seamless cloud login integration via Google OAuth to manage user subscriptions, bonus tokens, and synchronize premium features across devices.
- **Dynamic UI:** Features a modern, responsive user interface with real-time status updates for model downloading and OCR processing.

## 🛠️ Technology Stack

- **Frontend:** [Vue 3](https://vuejs.org/) (Composition API), [Vite](https://vitejs.dev/)
- **Backend/Desktop:** [Tauri](https://tauri.app/) (Rust)
- **Editor:** [Tiptap](https://tiptap.dev/)
- **Icons:** [Remix Icon](https://remixicon.com/)
- **Math Rendering:** [MathJax](https://www.mathjax.org/)

## 📦 Getting Started

### Prerequisites

Ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [Rust](https://www.rust-lang.org/tools/install)
- [Tauri Dependencies](https://tauri.app/v1/guides/getting-started/prerequisites) (Visual Studio C++ Build Tools for Windows)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ocr-editor-v3.git
   cd ocr-editor-v3
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

### Development

Start the development server with Hot Module Replacement (HMR):
```bash
npm run tauri dev
```

### Build for Production

To compile and bundle the application into standard desktop installers (e.g., `.msi` and `.exe` for Windows):
```bash
npm run tauri build
```
Once the build is complete, the installers will be available in the `src-tauri/target/release/bundle/` directory.

## 🔒 Privacy & Security

This application prioritizes user privacy. Core OCR functionalities are executed locally on your device, ensuring that sensitive documents and images are never uploaded to a third-party server unless you explicitly utilize cloud-based premium features.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
