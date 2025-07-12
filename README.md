# 🎨 RGB Color Guessing Game

[🔗 Live Demo](https://your-live-demo-url.com)  
*A fully playable version online!*


A fun color guessing game where you try to match a randomly chosen RGB value to its correct color square.

> ⚠️ **Note:** This game originally had a bug in Firefox where correct guesses weren't recognized. It’s now fixed using `getComputedStyle()` and proper color normalization in JavaScript.

---

## 🕹️ How to Play

1. You'll see an RGB color code like `rgb(255, 0, 0)` at the top of the page.
2. Click one of the color squares to guess which one matches the RGB code.
3. If you guess right – 🎉 “Correct!” will appear and all squares will change to that color.
4. If your guess is wrong, the square will disappear and you can try again.

---

## 🎯 Features

- **Difficulty Modes**:  
  - **Easy**: 3 color choices  
  - **Hard**: 6 color choices
- **Random Colors** every game
- **Play Again** button after a correct guess
- Responsive and lightweight

---

## 🛠 Built With

- HTML5
- CSS3
- Vanilla JavaScript

---

## 🐛 Fixed Firefox Compatibility

Previously, the game wouldn't recognize correct guesses in **Firefox** due to differences in how color values are read.

### 🔧 Fix Details:

- Replaced the unreliable:
  ```js
  var clickedColor = element.style.background;

  
