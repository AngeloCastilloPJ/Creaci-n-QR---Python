CREATION OF QR FOR ANY PAGE
Create QR for any page by copying the Python code into your virtual environment, be it Pycharm, Visual or any other.

1. You must previously install QRCODE -> pip install qrcode
2. You must copy the following code


import qrcode  as qr

img = qr.make("COLOCAR LA WEB AQUÍ")

img.save("wlinkdn_angelocp.png")


//Creación de QR con color de fondo y QR diferentes:

import qrcode
from PIL import Image

qr = qrcode.QRCode(version=1,
                   error_correction=qrcode.constants.ERROR_CORRECT_H,
                   box_size=10, border=4,)
qr.add_data("COLOCAR TU PÁGINA WEB")
qr.make(fit=True)
"""" Aquí deben colocar el color del Qr y del fondo"""
img = qr.make_image(fill_color="gold", back_colors="white")
img.save("elchebas.png")


