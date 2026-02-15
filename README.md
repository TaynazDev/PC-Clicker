# PC Clicker 🖥️

A fun and addictive incremental clicker game where you build your tech empire by clicking on PCs, buying upgrades, and unlocking special features!

## 🎮 Game Overview

PC Clicker is a browser-based incremental game built with React. Start by clicking on a motherboard to earn bits, then use those bits to purchase upgrades that automatically generate more bits. Build custom PCs, unlock powerful computers, and discover rare events that can skyrocket your progress!

## ✨ Features

### Core Gameplay
- **Click to Earn**: Click the motherboard to earn bits
- **Auto-Generation**: Purchase computers that automatically generate bits per second
- **Progressive Upgrades**: Unlock increasingly powerful computers as you earn more bits
- **Custom PC Builder**: Build custom PCs with various components (CPU, GPU, RAM, Storage, Motherboard, PSU, Case, Cooling)
- **Click Power Upgrades**: Increase bits earned per click with special upgrades

### Special Events
- **Dhahab Frenzy** (5% spawn chance): Click the flying golden PC to activate a 20-second power-up mode that doubles all production and transforms your computers into golden dhahabs
- **Threadripper Golden Ticket** (2% spawn chance): Click the rare flying CPU to instantly double your total bits

### Upgrade Systems
- **Base Computers**: Really Old PC, Raspberry Pi, Server, Data Center, Supercomputer, Quantum Computer, and the ultimate Everything Computer
- **Computer Overclockers**: Double the BPS of specific computer types (stacks multiplicatively)
- **Click Power Upgrades**: 6 upgrades from Better Mouse to Neural Interface
- **Custom PCs**: Build personalized computers with individual components

### Game Management
- **Auto-Save**: Game progress automatically saves to browser localStorage
- **Sell System**: Sell upgrades for 50% of their cost to optimize your strategy
- **Restart Option**: Reset your progress with a confirmation prompt

## 🚀 How to Play

### Getting Started
1. Open `index.html` in any modern web browser
2. Click the motherboard in the center to earn your first bits
3. Purchase your first upgrade when you have enough bits

### Basic Strategy
1. **Early Game**: Focus on click power upgrades and basic computers (Really Old PC, Raspberry Pi)
2. **Mid Game**: Build custom PCs and unlock Server/Data Center upgrades
3. **Late Game**: Purchase Supercomputers, Quantum Computers, and overclockers
4. **End Game**: Unlock the Everything Computer (10B bits) and maximize overclockers

### Tips
- Watch for flying golden dhahabs and threadrippers - they can significantly boost your progress
- Overclockers stack multiplicatively - 2 overclockers = 4x boost, 3 = 8x boost
- Selling upgrades refunds 50% of the cost - use this to optimize your build
- The Everything Computer stays hidden until you reach 10B bits or purchase it

## 📊 Stats Display

The left panel shows your real-time statistics:
- **Total Bits**: Your current currency
- **Bits Per Second**: Automatic generation rate
- **Bits Per Click**: Amount earned per click
- **Total Clicks**: Lifetime click counter

## 🛠️ Installation & Usage

### Play Locally
1. Clone or download this repository
2. Open `index.html` directly in your web browser
   - No build process or server required!
   - Works with direct file:// protocol

### Run with a Local Server (Optional)
```bash
# Using Python 3
python -m http.server 8080

# Using Python 2
python -m SimpleHTTPServer 8080

# Using Node.js (http-server)
npx http-server -p 8080
```
Then open `http://localhost:8080` in your browser.

## 🎨 Game Mechanics

### Computer Upgrades
Each computer tier generates bits per second:
- Really Old PC: 10 bps (5 bits)
- Raspberry Pi: 25 bps (50 bits)
- Server: 250 bps (5,000 bits)
- Data Center: 1,500 bps (30,000 bits)
- Supercomputer: 8,000 bps (150,000 bits)
- Quantum Computer: 100,000 bps (1,500,000 bits)
- Everything Computer: 50,000,000,000 bps (10,000,000,000 bits)

### Custom PC Components
Build custom PCs by purchasing:
- **CPU**: From AMD Athlon (80 bps) to AMD Ryzen 9 (1,200 bps)
- **GPU**: From Integrated Graphics (30 bps) to RTX 5090 (4,000 bps)
- **RAM**: From 4GB (20 bps) to 128GB (1,200 bps)
- **Storage**: From 128GB SSD (30 bps) to 8TB NVMe (1,200 bps)
- **Motherboard**: From Budget (40 bps) to Enthusiast (1,200 bps)
- **PSU**: From 400W (35 bps) to 1600W (1,200 bps)
- **Case**: From Basic Tower (15 bps) to Premium RGB Full Tower (560 bps)
- **Cooling**: From Stock Cooler (25 bps) to Custom Water Loop (1,200 bps)

### Click Power Upgrades
Boost your clicking power:
- Better Mouse: +1 bpc (50 bits)
- Auto-Clicker Software: +5 bpc (250 bits)
- Mechanical Keyboard: +25 bpc (1,000 bits)
- Gaming Setup: +100 bpc (5,000 bits)
- AI Clicking Assistant: +500 bpc (25,000 bits)
- Neural Interface: +2,500 bpc (100,000 bits)

### Overclocker System
Purchase overclockers to double computer production:
- Each overclocker costs double the previous one
- Multiple overclockers stack multiplicatively (2x, 4x, 8x, 16x, etc.)
- Available for all computer types once purchased

## 📁 Project Structure

```
PC-Clicker/
├── index.html          # Main game file (HTML, CSS, and React code)
├── assets/
│   └── images/        # All game images
│       ├── 36013.gif             # Animated background
│       ├── motherboard.webp      # Main clickable motherboard
│       ├── dhahab.png            # Golden PC for frenzy mode
│       ├── dhahab pc.png         # Golden PC transformation
│       ├── threadripper.png      # Rare CPU event
│       ├── everything.png        # Ultimate endgame computer
│       ├── hmm.png               # Hidden upgrade placeholder
│       ├── really old pc.png     # First computer upgrade
│       ├── raspberry pi.png      # Early game upgrade
│       ├── server.png            # Mid game upgrade
│       ├── data centre.png       # Mid-late game upgrade
│       ├── supercomputer.png     # Late game upgrade
│       ├── qantum computer.png   # End game upgrade
│       ├── basic tower.png       # PC case option
│       ├── mid tower.png         # PC case option
│       ├── mid tower with rgb.png # PC case option
│       ├── full tower.png        # PC case option
│       ├── full tower with rgb.png # PC case option
│       └── premium rgb full tower.png # PC case option
├── CHANGELOG.md       # Detailed version history and updates
├── LICENSE            # MIT License
└── README.md          # This file
```

## 🔧 Technical Details

- **Framework**: React 18 (via CDN)
- **Styling**: Pure CSS with animations
- **Storage**: Browser localStorage for game saves
- **Compatibility**: Works in all modern browsers (Chrome, Firefox, Safari, Edge)
- **No Build Required**: Single HTML file with inline JavaScript

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Copyright (c) 2026 TaynazDev

## 🎯 Future Ideas

- Achievements system
- Prestige/rebirth mechanics
- More special events
- Sound effects and music
- Mobile-optimized UI
- Multiplayer leaderboards
- Dark/Light theme toggle

## 🐛 Known Issues

- Custom PC tooltips may overflow on smaller screens
- Game saves are browser-specific (won't transfer between browsers)

## 🤝 Contributing

Feel free to fork this project and submit pull requests! Some areas for contribution:
- Bug fixes
- New features
- Performance improvements
- UI/UX enhancements
- Documentation improvements

## 📞 Contact

Created by TaynazDev - Feel free to reach out with feedback or suggestions!

## 🎮 Have Fun!

Enjoy building your tech empire! Remember, it's all about patience, strategy, and clicking that motherboard! 🖱️💻
