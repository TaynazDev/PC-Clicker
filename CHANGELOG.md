# PC Clicker - Change Log

## Latest Updates - February 12, 2026

### New Features
- **Custom PC Overclocker** - Added overclocker upgrade for Custom PC builds
  - Costs 5,000 bits (balanced between Raspberry Pi and Server overclockers)
  - Doubles Custom PC production with each purchase
  - Stacks multiplicatively like other overclockers

---

## Previous Updates - February 10, 2026

### Bug Fixes
- **Fixed image loading issues when opening HTML directly (without live server)**
  - Added explicit relative paths (./) to all image references
  - URL-encoded spaces in image filenames (%20) for browser compatibility
  - Now works correctly when opening index.html directly in any browser

---

## Previous Updates - February 10, 2026

### Major New Features
- **Dhahab Frenzy System** - Rare golden PC that triggers a 20-second power-up mode
  - Flying dhahab.png appears with 5% spawn chance every 3 seconds
  - Clicking it activates frenzy mode with 2x multiplier to all production
  - During frenzy: motherboard transforms to dhahab pc.png
  - All owned computers display as golden dhahab PCs
  - Continuous rain of golden dhahabs throughout frenzy duration
  - Visual effects: golden overlay, pulsing borders, and countdown timer

- **Threadripper Golden Ticket** - Ultra-rare flying CPU that doubles your wealth
  - 2% spawn chance every 3 seconds
  - Flies from opposite direction (right to left) with red glow
  - Clicking doubles your total bits instantly
  - Shows threadripper.png in click effect

- **Everything Computer** - Ultimate endgame upgrade
  - Costs 10.0B bits (10 billion)
  - Produces 50.0B bits per second
  - Hidden as "???" with hmm.png until you reach 10B bits (or buy it)
  - Stays revealed permanently once unlocked

- **Computer Overclocker System** - New upgrade category to boost production
  - 7 overclockers for each computer type (Raspberry Pi, Really Old PC, Server, Data Center, Supercomputer, Quantum, Everything)
  - Each overclocker doubles the BPS of its target computer
  - Stacks multiplicatively (2 overclockers = 4x, 3 = 8x, etc.)
  - Price doubles after each purchase (exponential cost scaling)
  - Requires owning the target computer to purchase
  - Everything Overclocker hidden until Everything is bought

### Gameplay Changes
- **Frenzy Multiplier**: Changed from flat +1M bonuses to 2x multiplier (scales with progress)
  - Bits per click: 2x during frenzy
  - Bits per second: 2x during frenzy
- **Threadripper**: Changed from flat +1B bits to doubling total bits (scales with progress)
- **Shop Reorganization**: "UPGRADES" section renamed to "COMPUTERS"

### Visual Improvements
- Frenzy notification displays dhahab.png icons instead of star emojis
- Raining dhahab particles with spinning fall animation
- Golden glow effects and pulsing animations during frenzy
- Improved click effect system - shows appropriate image based on what was clicked
- Overclocker multiplier display (x2, x4, x8, etc.)

### Bug Fixes
- Fixed overclockers not being cleared on game restart
- Fixed click effects showing wrong images for special events
- Fixed display values for bits per click and bits per second during frenzy
- Fixed upgrade sprites showing hmm.png unintentionally

### Technical Improvements
- Added overclockerUpgrades state management
- Updated save/load system to include overclocker progress
- Improved click effect tracking with image property
- Enhanced spawn rate tuning for special events

## Previous Updates

### New Features
- **Sell Upgrades** - You can now sell any upgrade (Click Power, Base Upgrades, or Custom PCs) for 50% of their cost
  - Sell buttons appear below buy buttons when you own at least one upgrade
  - Selling reduces the upgrade count and refunds bits
  - Useful for optimizing your build or recovering bits from early purchases

### Bug Fixes
- Fixed sell price calculation to prevent upgrade costs from going below base price
- Upgrade costs now properly maintain minimum base cost when selling

### Visual Improvements
- Added animated GIF background (36013.gif) with adjustable transparency overlay
- Replaced center PC sprite with clickable motherboard image (motherboard.webp)
- Added rounded frame with green border around the motherboard
- Small motherboard images now fly upward when clicking
- Removed grid pattern from game world for cleaner look
- Added images to all case options in PC builder
- Added images to base upgrades (Really Old PC, Raspberry Pi, Server, Data Center, Supercomputer, Quantum Computer)

### New Features
- **Click Power Upgrade System** - 6 new upgrades to increase bits per click:
  - Better Mouse (+1 bit/click) - 50 bits
  - Auto-Clicker Software (+5 bits/click) - 250 bits
  - Mechanical Keyboard (+25 bits/click) - 1,000 bits
  - Gaming Setup (+100 bits/click) - 5,000 bits
  - AI Clicking Assistant (+500 bits/click) - 25,000 bits
  - Neural Interface (+2,500 bits/click) - 100,000 bits
- **Restart Button** - Reset game progress with confirmation prompt
- **Custom PC Tooltips** - Hover over custom PCs to see all parts and their individual BPS contributions
- **Part Price Scaling** - PC parts now increase in price (15%) each time purchased
- **Raspberry Pi** - New upgrade between Really Old PC and Custom PC (50 bits, 25 bps)

### Gameplay Changes
- **Increased Income (10x multiplier)**:
  - Really Old PC: 1 → 10 bps
  - Raspberry Pi: 2 → 25 bps
  - Server: 25 → 250 bps
  - Data Center: 150 → 1,500 bps
  - Supercomputer: 800 → 8,000 bps
  - Quantum Computer: 10,000 → 100,000 bps

- **PC Parts BPS Increased (8x average)**:
  - All CPUs, GPUs, RAM, Storage, Motherboards, PSUs, Cases, and Cooling components significantly buffed
  - Example: AMD Ryzen 9 now gives 1,200 bps (was 150)
  - Example: RTX 5090 now gives 4,000 bps (was 500)

- **Increased upgrade costs**:
  - Server: 2,000 → 5,000 bits
  - Data Center: 10,000 → 30,000 bits
  - Supercomputer: 50,000 → 150,000 bits
  - Quantum Computer: 500,000 → 1,500,000 bits

### Content Changes
- Removed Workstation upgrade
- Removed Mid Tower with Glass case option
- Swapped RGB Mid Tower and Full Tower positions in builder
- Changed all Intel CPUs to AMD equivalents:
  - Intel Celeron → AMD Athlon
  - Intel i3/i5/i7/i9 → AMD Ryzen 3/5/7/9

### UI Improvements
- Added "BITS PER CLICK" stat display in left panel
- Custom PCs now display individually in shop with case images
- Each custom PC shows as separate item in inventory with its case image
- Improved custom PC tooltips showing component breakdown
- Click effects now show actual bits earned

### Technical Improvements
- All game state saved to localStorage (bits, upgrades, click upgrades, custom PCs, part purchase counts)
- Part prices dynamically calculated based on purchase history
- Custom PC purchase tracking for price scaling

## Known Issues
- Custom PC tooltips may overflow on smaller screens
- Images with spaces in filenames work correctly with proper path handling
