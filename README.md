CREATION OF QR FOR ANY PAGE
Create QR for any page by copying the Python code into your virtual environment, be it Pycharm, Visual or any other.

1. You must previously install QRCODE -> pip install qrcode
2. You must copy the following code


import qrcode  as qr

img = qr.make("COLOCAR LA WEB AQUÍ")

img.save("wlinkdn_angelocp.png")

