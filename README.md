# QR Code Generator 🔲

A beginner-friendly Python project that generates customized QR codes using the `qrcode` and `Pillow` libraries.

---

## 📌 Features

- Create QR codes from any text or link
- Customize colors (foreground and background)
- Set size, border, and error correction level
- Export the result as a `.png` image

---

## 📂 Project Files

| File Name             | Description                          |
|-----------------------|--------------------------------------|
| `qr_code_generator.py`| Main Python script to generate QR    |
| `qr.png`            | Output image (after you run script)  |

---

## 💻 Requirements

Make sure Python is installed.

Install required libraries with:
```bash
pip install qrcode[pil]


```
## 🚀 How to Run
Download the qr_code_generator.py file

Open terminal / CMD in that folder

```bash
python qr_code_generator.py
```

### 🧠 Code Overview

```bash
import qrcode
from PIL import Image

qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_H,
    box_size=20,
    border=2,
)

qr.add_data("don")
qr.make(fit=True)
img = qr.make_image(fill_color="white", back_color="gray")
img.save("Luck.png")
```

You can change "don" to anything (your name, URL, etc.)


## 🧑‍💻 Author

Jashandeep
Aspiring Cybersecurity Student | Tech Learner

📫 [https://www.linkedin.com/in/jashandeepsaroha/]



