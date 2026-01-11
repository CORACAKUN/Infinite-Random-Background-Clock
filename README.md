# Infinite Random Background Clock

A lightweight web project that displays a real-time digital clock with milliseconds and the current date while continuously loading random fullscreen background images.  
Built using pure HTML, CSS, and JavaScript with no external libraries.

---

## Features

- Real-time digital clock with milliseconds
- Live date display (weekday, month, day, year)
- Infinite random fullscreen background images
- Preloaded image queue to avoid flicker
- Responsive layout that adapts to screen size
- Smooth background transitions
- Runs entirely in the browser

---

## Preview

Open `index.html` in a browser to see a fullscreen clock with constantly changing random backgrounds.

---

## Project Structure

```
infinite-random-background-clock/
│
├── index.html
└── README.md
```

---

## Getting Started

### Run Locally

1. Download or clone this repository
2. Open `index.html` in any modern web browser
3. The clock and background system will start automatically

No installation, server, or build tools are required.

---

## Built With

- HTML5
- CSS3
- JavaScript (Vanilla)

---

## How It Works

### Clock System
- Uses `requestAnimationFrame` for smooth millisecond updates
- Displays time in HH:MM:SS.mmm format
- Date is formatted using `toLocaleDateString`

### Background Image System
- Random images are loaded from `picsum.photos`
- Images are preloaded into a queue
- A Set prevents duplicate image reuse
- Background changes every second without visible loading delays

---

## Customization

### Change Background Interval
```js
setInterval(changeBackground, 1000);
```
Increase the value to slow down background changes.

### Adjust Clock Format
Modify the time and date formatting inside the `update()` function.

### Change Font and Styling
Edit the CSS rules for `#clock` and `#date`.

---

## Browser Support

- Google Chrome
- Microsoft Edge
- Firefox
- Safari
- Mobile browsers (Android and iOS)

An active internet connection is required for background images.

---

## Learning Purpose

This project demonstrates:
- High-precision time rendering in JavaScript
- Efficient background image preloading
- DOM updates using `requestAnimationFrame`
- Responsive fullscreen layouts
- Clean separation of logic and styling

---

## License

This project is open-source and free to use for learning and personal projects.
