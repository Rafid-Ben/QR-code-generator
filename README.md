# QR Code Generator

## Description
This project is a simple Python script to generate QR codes with customizable parameters. It allows users to encode text or URLs into QR codes and save them as image files.

## Features
- Generate QR codes from any text or URL
- Customize the QR code version, error correction level, box size, and border
- Save the QR code as an image file

## Error Correction Levels

The error correction level in QR codes determines how much data can be recovered if the code is damaged or partially obscured. There are four levels of error correction:

- **L (Low)**: Recovers up to 7% of the data. Suitable for scenarios where the QR code is expected to remain clean and undamaged.
- **M (Medium)**: Recovers up to 15% of the data. A good default for general use cases, balancing data capacity and error correction.
- **Q (Quartile)**: Recovers up to 25% of the data. Ideal for scenarios where the QR code may experience moderate damage or wear.
- **H (High)**: Recovers up to 30% of the data. Best for scenarios where the QR code may be heavily damaged or needs maximum reliability.

In the script, the error correction level is set using `qrcode.constants.ERROR_CORRECT_L`. You can adjust this value as needed to suit your requirements.


## Installation
To use this project, you need to have Python installed. You can install the required package using pip:

```bash
pip install qrcode[pil]

