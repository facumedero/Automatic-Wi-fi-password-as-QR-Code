# Automatic-Wi-fi-password-as-QR-Code

## Requisites
pip install wifi_qrcode_generator

## Code
import wifi_qrcode_generator as qr
qr.wifi_qrcode('wifi name', False,'WPA', 'password')

import pyqrcode

from PIL import Image

link = input("Enter anything to generate QR : ")

qr_code = pyqrcode.create(link)

qr_code.png("QRCode.png", scale=5)

Image.open("QRCode.png")
