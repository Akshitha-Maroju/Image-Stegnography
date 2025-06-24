# Image-Stegnography

This project demonstrates **image steganography** — the art of hiding secret text messages inside images — using Python and an interactive **Gradio** interface. You can encode a hidden message into an image and decode it back using this tool. Built and tested in **Google Colab**.

---

## 🚀 Features

- 📤 Upload any `.png` image
- 📝 Enter secret text to hide
- 🖼️ View and download the encoded image
- 🔍 Upload the encoded image to decode the message
- 🧠 Built with Python, Pillow, and Gradio
- ✅ 100% Google Colab compatible

---

## 🧰 Tech Stack

- `Python 3.10+`
- `Gradio` for GUI
- `Pillow` for image processing

---

## 🔧 How It Works

- Each character in the secret message is converted to **8-bit binary**.
- Bits are hidden in the **least significant bits (LSB)** of RGB pixels.
- A unique delimiter `###` is added at the end to mark the finish of the hidden message.
- The decoding process reads LSBs to reconstruct the hidden message until it hits the delimiter.

---

## 📁 Usage in Google Colab

1. **Open the Colab notebook**  
2. Install required libraries (Gradio, Pillow)  
3. Run the code cells  
4. Upload an image and enter a secret message  
5. Click **"Encode"** to get a stego-image  
6. Use **"Decode"** tab to retrieve the hidden message  


