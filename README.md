# ⚡ 3D Reaction Timer Game

A modern, interactive web-based reaction timer game featuring Three.js 3D graphics. Test your reflexes by clicking a rotating 3D dodecahedron as quickly as possible after it turns green!

![Game Preview](https://img.shields.io/badge/Status-Production%20Ready-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?logo=three.js&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🎮 Features

### Core Gameplay
- **3D Graphics**: Stunning dodecahedron shape with multi-axis rotation and smooth animations
- **Precise Timing**: Millisecond-accurate reaction time measurement
- **Random Delays**: 1-5 second random wait periods to prevent prediction
- **False Start Detection**: Penalty system for clicking too early
- **Performance Tracking**: Real-time statistics including best time and average
- **Multiple Controls**: Start rounds with mouse click or spacebar

### Visual Design
- **Modern UI**: Clean, contemporary design with glassmorphic elements
- **Color-Coded Feedback**: Performance ratings with distinct color schemes
  - 🔴 Amazing (< 200ms)
  - 🟠 Very Good (200-250ms)
  - 🟢 Good (250-300ms)
  - 🔵 Average (300-400ms)
  - ⚪ Below Average (> 400ms)
- **Real-time Score Display**: Top-right overlay showing current performance
- **Responsive Design**: Optimized for desktop and mobile devices

### Technical Features
- **Three.js Integration**: Professional 3D rendering with r128
- **Raycasting**: Accurate click detection on 3D objects
- **State Management**: Clean game state architecture
- **Performance Optimized**: Efficient animation loop with capped pixel ratio
- **Accessibility**: Large click targets and keyboard support

## 🚀 Quick Start

### Option 1: Direct Use
1. Download `reaction-timer.html`
2. Download `favicon.png` (optional)
3. Open `reaction-timer.html` in any modern web browser
4. Start playing!

## 📖 How to Play
1. **Start a Round**
   - Click the "Start Round" button, or
   - Press the **SPACEBAR**

2. **Wait for Green**
   - The 3D shape will appear amber (yellow)
   - Wait patiently for it to turn green
   - Don't click too early or you'll get a false start!

3. **React Quickly**
   - When the shape turns green, click it as fast as possible
   - Your reaction time will be displayed immediately

4. **Track Progress**
   - View your performance rating in the top-right corner
   - Check your statistics: rounds played, best time, and average

5. **Improve Your Score**
   - Keep playing to improve your reaction time
   - Aim for under 200ms for an "Amazing" rating!

## 🎯 Performance Ratings

| Rating | Time Range | Color | Description |
|--------|-----------|-------|-------------|
| **Amazing** | < 200ms | Red | Lightning-fast reflexes! 🔥 |
| **Very Good** | 200-250ms | Amber | Excellent reaction time! ⚡ |
| **Good** | 250-300ms | Green | Great performance! ✨ |
| **Average** | 300-400ms | Blue | Solid effort! 👍 |
| **Below Average** | > 400ms | Gray | Keep practicing! 💪 |

## 🛠️ Technical Stack

- **HTML5** - Semantic structure
- **CSS3** - Modern styling with flexbox/grid, gradients, and animations
- **Vanilla JavaScript** - No frameworks, pure ES6+
- **Three.js r128** - 3D graphics rendering
- **Google Fonts** - Inter & Space Grotesk typography

## 📁 Project Structure

```
reaction-timer-game/
│
├── index.html        # Main game file 
├── favicon.png       # Game icon 
└── README.md         # This file
```

## 🎨 Design System

### Color Palette
- **Background**: `#0F172A` (Deep Slate)
- **Primary Accent**: `#10B981` (Emerald Green)
- **Warning**: `#F59E0B` (Amber)
- **Error**: `#EF4444` (Red)
- **Text Primary**: `#F8FAFC` (Off-white)
- **Text Secondary**: `#94A3B8` (Slate Gray)
- **Surface**: `#1E293B` (Lighter Slate)

### Typography
- **Primary Font**: Inter (weights: 400, 600)
- **Accent Font**: Space Grotesk (weights: 500, 700)

## 🌐 Browser Compatibility

Tested and working on:
- ✅ Chrome/Edge (v90+)
- ✅ Firefox (v88+)
- ✅ Safari (v14+)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

**Requirements:**
- WebGL support
- ES6+ JavaScript support
- Modern CSS support (flexbox, grid, gradients)

## 📱 Mobile Optimization

- Responsive canvas sizing (400px on mobile, 500px on desktop)
- Compact score overlay on smaller screens
- Touch-friendly click targets
- Optimized performance for mobile devices

## 🔧 Customization

### Modify Delay Range
```javascript
// In startRound() function, change this line:
const delay = 1000 + Math.random() * 4000; // Currently 1-5 seconds

// Example: 2-6 seconds
const delay = 2000 + Math.random() * 4000;
```

### Change Shape
```javascript
// Replace DodecahedronGeometry with another shape:
const mainGeometry = new THREE.IcosahedronGeometry(1.5, 0); // 20-sided
// or
const mainGeometry = new THREE.OctahedronGeometry(1.5, 0); // 8-sided
```

### Adjust Colors
```css
/* In the <style> section, modify CSS variables */
/* For example, change primary accent: */
background: linear-gradient(135deg, #3B82F6 0%, #2563EB 100%); /* Blue theme */
```

## 🎓 Educational Use

This project demonstrates:
- **3D Graphics Programming**: Three.js scene setup, lighting, and rendering
- **Game Development**: State management, timing systems, user input handling
- **Web Development**: Modern HTML/CSS/JS, responsive design, UX principles
- **Performance Optimization**: Efficient animation loops, raycasting, cleanup

Perfect for:
- Frontend development portfolios
- JavaScript/Three.js learning projects
- Game development tutorials
- Web graphics demonstrations

## 🐛 Known Issues

- None currently reported

## 👨‍💻 Author

Created as a portfolio demonstration project showcasing modern frontend development skills.

## 🤝 Contributing

Feel free to fork, modify, and improve! Suggestions for enhancements:
- Add sound effects
- Implement difficulty levels
- Create global leaderboards
- Add different game modes
- Implement achievements/badges

## 📊 Future Enhancements

- [ ] Sound effects for game events
- [ ] Multiple difficulty levels
- [ ] Different 3D shapes to choose from
- [ ] Dark/light theme toggle
- [ ] Save high scores to local storage
- [ ] Multiplayer mode
- [ ] Mobile app version

## 💡 Tips for Best Performance

1. **Focus**: Keep your eyes on the shape
2. **Anticipation**: Don't try to predict - wait for the green
3. **Relaxation**: Tension slows reactions - stay relaxed
4. **Practice**: Reaction time improves with regular practice
5. **Environment**: Use a mouse for best accuracy (touchpad can be slower)

## 🙏 Acknowledgments

- **Three.js** - For the excellent 3D graphics library
- **Google Fonts** - For beautiful typography
- **CDNjs** - For reliable CDN hosting

---

**Ready to test your reflexes? Open the game and see if you can achieve an "Amazing" rating! ⚡**

*Average human reaction time: 200-300ms | Professional gamers: 150-200ms | Can you beat them?*