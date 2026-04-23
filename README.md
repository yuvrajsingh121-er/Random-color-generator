# Random-color-generator

# 🎨 Random Color Generator

Ek simple aur interactive JavaScript project jo click karne par random hex colors generate karta hai aur unhe background par apply karta hai.

---

## 🧐 Overview

Yeh project beginner-friendly hai aur Vanilla JavaScript ke DOM manipulation aur Math functions ko samajhne ke liye behtareen hai. Iska istemal aap apne web projects mein dynamic themes banane ke liye kar sakte hain.

## 🚀 Live Demo

Aap is project ka live preview yahan dekh sakte hain:
**[Apna Vercel ya GitHub Pages ka link yahan dalein]**

## ✨ Features

* **Random Hex Generation:** Har click par ek unique hex code.
* **Visual Feedback:** Page ka background color turant change hota hai.
* **Copy to Clipboard:** (Optional) Hex code ko copy karne ka feature.
* **Responsive Design:** Mobile aur Desktop dono par sahi chalta hai.

## 🛠️ Tech Stack

* **HTML5**
* **CSS3** (Custom Properties / Flexbox)
* **JavaScript** (ES6+)

## 📖 Logic Kaise Kaam Karta Hai?

Iska core logic `Math.random()` function par base hai:

$$color\_code = \# + (16^{6} \text{ combinations of hexadecimal values})$$

```javascript
function getColor() {
  const randomNumber = Math.floor(Math.random() * 16777215);
  const randomCode = "#" + randomNumber.toString(16);
  document.body.style.backgroundColor = randomCode;
}
