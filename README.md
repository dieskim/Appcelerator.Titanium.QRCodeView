# Appcelerator.Titanium.QRCodeView
Appcelerator Titanium QR Code Generator that returns a Ti.UI.ImageView containing the QR code Image 
- iOS/Android support!


- This Appcelerator module is a work in progress
- Please log issues via Github issues
- Any pull requests and suggestions welcome!
- Packaged By: Dieskim of (dieskim.me)](https://www.dieskim.me)


## Installation:
1. Git Clone (Download and Copy the qrcode.js file) to your `lib/` (Alloy) or your Resources (Classic) directory

## How to use:
```
// require qrcode and spesify text and errorCorrectLevel
var qrcode = require('qrcode').QRCode({
	text: 'https://github.com/k0sukey/TiQRCodeView',		// text string for QR code
	errorCorrectLevel: 'M'					// Possible Values: L / M / Q / H
});


// create Ti.UI.ImageView qrcodeView - spesify width, height and margin
var qrcodeView = qrcode.createQRCodeView({
	width: 300,
	height: 300,
	margin: 4,
});

// add qrcodeView to youViewNameHere
youViewNameHere.add(qrcodeView);

```


### Original
TiQRCodeView by Kosuke Isobe (https://github.com/k0sukey)  - https://github.com/k0sukey/TiQRCodeView

### Additions
Christian Moss - (https://github.com/mandelmonkey) - https://github.com/IndieSquare/TiQRCodeView

### Based on
QR Code Generator for JavaScript 
- Copyright (c) 2009 Kazuhiko Arase (http://www.d-project.com) 
- Licensed under the MIT license - http://www.opensource.org/licenses/mit-license.php
The word 'QR Code' is registered trademark of DENSO WAVE INCORPORATED - http://www.denso-wave.com/qrcode/faqpatent-e.html
