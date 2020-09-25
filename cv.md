YAN SOLONOVICH
---
#### Junior JS Developer

###### Home Address:
Minsk, Tikotsky street, build 42, flat 45, 220119, BY

###### Phone:
+375 (29) 197 60 78

###### E-mail:
solonovichyan@gmail.com

###### Telegram:
@solonovich_yan

#### SKILLS

C++, HTML, CSS, JS, Node.JS, Lua, MySQL.
SolidWorks, Altium Designer, Photoshop, KeyShot.

#### CODE EXAMPLES

[My current project](https://noexanu.github.io/web/)

```javascript
function SET_COLOR(R, G, B, x, y, boxSize) {
	let OUT_R = R, OUT_G = G, OUT_B = B;
	let stepYR = boxSize.height / (OUT_R + 1);
	for (let t = 0; y > t + stepYR; t = t + stepYR) {
		if (OUT_R > 0) {
			OUT_R--;
		}
	}
	let stepYG = boxSize.height / (OUT_G + 1);
	for (let t = 0; y > t + stepYG; t = t + stepYG) {
		if (OUT_G > 0) {
			OUT_G--;
		}
	}
	let stepYB = boxSize.height / (OUT_B + 1);
	for (let t = 0; y > t + stepYB; t = t + stepYB) {
		if (OUT_B > 0) {
			OUT_B--;
		}
	}
	let MAX = Math.max(OUT_R, OUT_G, OUT_B);
	let stepXR = boxSize.width / (MAX - OUT_R + 1);
	for (let t = 0; x > t + stepXR; t = t + stepXR) {
		if (OUT_R < 255) {
			OUT_R++;
		}
	}
	let stepXG = boxSize.width / (MAX - OUT_G + 1);
	for (let t = 0; x > t + stepXG; t = t + stepXG) {
		if (OUT_G < 255) {
			OUT_G++;
		}
	}
	let stepXB = boxSize.width / (MAX - OUT_B + 1);
	for (let t = 0; x > t + stepXB; t = t + stepXB) {
		if (OUT_B < 255) {
			OUT_B++;
		}
	}
	return [OUT_R, OUT_G, OUT_B]
}



function HUE_COLOR_PICKER(ID) {
	let R = 255, G = 0, B = 0;
	for (let t = 0; t < document.getElementById("HUE" + ID).value; t++) {
		if (t < 255) {
			G++;
		}
		if (t > 255 && t < 511) {
			R--;
		}
		if (t > 511 && t < 767) {
			B++;
		}
		if (t > 767 && t < 1023) {
			G--;
		}
		if (t > 1023 && t < 1279) {
			R++;
		}
		if (t > 1279) {
			B--;
		}
	}
	return [R, G, B];
}



function HEXtoRGB(HEX) {
	let R, G, B;
	if (HEX.length == 4) {
		return [
   			R = parseInt(HEX.slice(1, 2), 16),
			G = parseInt(HEX.slice(2, 3), 16),
			B = parseInt(HEX.slice(3, 4), 16)
  		];
	}
	else{
		return [
   			R = parseInt(HEX.slice(1, 3), 16),
			G = parseInt(HEX.slice(3, 5), 16),
			B = parseInt(HEX.slice(5, 7), 16)
  		];
	}
}



function RGBtoHEX(R, G, B) {
	return ("#" + ((1 << 24) + (R << 16) + (G << 8) + B).toString(16).slice(1));
}
```

#### WORK EXPERIENCE

NaN

#### EDUCATION

* 2014-09 – 2018-07
BUSIR affiliate “Minsk Radioengineering College”
Thesis title: “Microprocessor-controlled audio power amplifier repair and adjustment guid”
Thesis supervisor: Docent Boris Danilenko

* 2018-09 – Present
Belarusian State University of Informatics and Radioelectronics

#### LANGUAGES

English, Русский, Беларуская.
English level – A2+ (tested by EPAM Training Center).
