# python_project_QR-CODE

QR Code Generator | Python

This is a simple Python project that allows you to generate QR codes from any URL.
The generated QR code is saved as a PNG image file.

📌 Features

Enter any URL and convert it into a QR code

Automatically saves the QR code as a .png file

If the file name does not include .png, it will be added automatically

Very easy to use and beginner-friendly

🧩 How It Works

The project uses the qrcode library in Python to generate QR codes.

✔️ Install Required Library
pip install qrcode[pil]

✔️ Python Code
import qrcode

url = input("enter your url:")
filename = input("filename you want to save it as:")

if not(filename.endswith(".png")):
    filename = filename + ".png"

img = qrcode.make(url)
img.save(filename)
print(f"QR code saved as {filename}")

▶️ How to Run

Clone or download the project

Open a terminal in the project folder

Run:

python qr_generator.py


Enter your URL

Enter the file name

Your QR code will be saved in the same folder 🎉

📂 Output Example

Input URL → https://google.com

File name → google_qr

Saved as → google_qr.png

📸 Sample Result

The script generates a clean QR PNG image like this:

[QR Code Image Generated]
