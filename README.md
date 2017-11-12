# QR Code generator for OpenSCAD

This project can generate [OpenSCAD](http://www.openscad.org/) source code for a QR code encoding given value. There are already [two](https://www.thingiverse.com/thing:258542) [projects](https://www.thingiverse.com/thing:46884) on Thingiverse, but the first does not work properly and the second requires running executable on your machine. So I created third one.

## How it works

This project works completely online in JavaScript. Go to https://ridercz.github.io/OpenSCAD-QR/ and enter the value of your code. The page will generate image of your code (so you can check it's working) and also OpenSCAD code, which will create array with `0` and `1`, representing the code. 

Also provided is simple OpenSCAD module (method) `qr_render` for drawing the encoded QR Code with given parameters:
* `module_size` - the size of single square, default 1x1 mm
* `height` - extrusion height, default 1 mm

The resulting code is not intended to be used 'as is', you are supposed to incorporate it to your own models. For example see the [QR Code Dog Tag](https://www.thingiverse.com/thing:2640021)

## Acknowledgements

The heavy lifting - QR Code generation itself - was done by the perfect [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) by Kazuhiko Arase. I just added OpenSCAD code generation and simple web interface.

## Author

Developed by *Michal Altair Valášek*. For more information see:
* https://www.rider.cz/
* https://www.altairis.cz/
* https://keybase.io/ridercz/
* https://twitter.com/ridercz/
* https://facebook.com/rider.cz/

This work is licensed under terms of the [MIT License](LICENSE).