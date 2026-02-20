# PC Clicker - Change Log

## Latest Updates - February 20, 2026

### Milestone System - Achievement Tracking 🏆
- **40 Punny Milestones Across 5 Categories** - Track your progress with humor!
  - **Progress Milestones (12)**: Track total clicks, lifetime bits, and BPS achievements
    - "Click to the Future" (1K clicks) - *"Great Scott! That's a lot of clicking!"*
    - "Bit of a Problem" (1B lifetime bits) - *"That's byte-sized dedication!"*
    - "Core Values" (1M BPS) - *"Your CPU cores are working overtime!"*
  - **Collection Milestones (9)**: Computer ownership and custom PC building goals
    - "Computer Hoarder" (50 computers) - *"At this point, just open a Best Buy"*
    - "Custom Built Different" (1 custom PC) - *"Cable management not included"*
    - "RGB Everything" (25 custom PCs) - *"If it doesn't glow, it doesn't go!"*
  - **Event Milestones (8)**: Special event interaction tracking
    - "Supply and Demand Issues" (10 supply chains) - *"Sheesh, the supply company must be really bad"*
    - "Dhahab Digger" (10 Dhahaballoons) - *"That's some serious gold mining!"*
    - "Thread the Needle" (1 Threadripper) - *"You've got some serious thread count"*
  - **Upgrade Milestones (3)**: Overclocker purchase milestones
    - "Thermal Paste Enthusiast" (50 overclockers) - *"You buy it in bulk now, don't you?"*
  - **Economy Milestones (8)**: Buying and selling achievements
    - "Penny Pincher" (1 sale) - *"One person's trash is... still your trash"*
    - "eBay Power Seller" (200 sales) - *"Buy high, sell low! Wait..."*

- **Milestone UI Features**
  - **🏆 View Milestones Button** in shop panel showing completion count (X/40)
  - **Milestone Modal** with category filtering (All, Progress, Collection, Events, Upgrades, Economy)
  - **Animated Popup Notifications** when milestones are completed
  - **Hidden Descriptions** on locked milestones - reveals the pun on completion!
  - **Beautiful Visual Design** with golden gradients for completed achievements

- **Lifetime Stats Tracking**
  - Tracks: Total clicks, lifetime bits earned, Dhahab clicks, Threadripper clicks
  - Monitors: Supply chains survived, total purchases, total sales, custom PCs built
  - Stats persist through gameplay and save/load
  - All progress resets with "Restart Game" button

---

## Previous Updates - February 20, 2026

### Supply Chain Event Enhancements
- **Increased Supply Chain Severity** - Major changes to make the event more impactful
  - **Complete Production Halt**: Changed from 50% reduction to 0% - all production stops
  - **Motherboard Disabled**: PC is now unclickable during supply chain issues
    - Visual feedback: 50% opacity and "not-allowed" cursor
    - Prevents all manual clicking
  - **UI Indicators**: Bits per click displays 0 during the event
  - **Complete Red Theme**: All UI elements now turn red
    - Zoom controls turn red
    - Owned upgrades display borders (left/right) turn red
    - All panels, buttons, and borders affected
  - **Updated Notification**: Message changed from "Production reduced by 50%" to "All production HALTED"

---

## Previous Updates - February 20, 2026

### New Features
- **User-Adjustable Zoom Controls** - Added zoom controls to adapt to different screen sizes and display scaling
  - Located in the left stats panel below the restart button
  - **Zoom In/Out buttons** (+/-) to adjust from 50% to 150%
  - **Reset button** to return to 100% zoom
  - **Persistent zoom** - Saves preference in localStorage
  - **Smooth transitions** when zooming
  - **Auto-hidden** on mobile devices (768px and below)
  - Perfect for laptops with Windows display scaling enabled

### UI Improvements
- **Enhanced Responsive Design** - Added more breakpoints for better laptop support
  - Multiple laptop breakpoints: 1600px, 1440px, 1366px, 1280px
  - Height-based media queries for laptops with limited vertical space (900px, 768px)
  - Better scaling across different laptop resolutions

---

## Previous Updates - February 15, 2026

### New Features
- **Responsive Design** - Game now adapts to different screen sizes and devices
  - **Tablet Support (up to 1024px)**: Optimized panel sizes and spacing
  - **Mobile Tablet (up to 768px)**: Reorganized layout with stats on top, shop on bottom
  - **Mobile Phone (up to 480px)**: Compact design with touch-friendly elements
  - All text, buttons, and UI elements scale appropriately
  - PC builder modal adapts to smaller screens
  - Maintained visual style across all device sizes

### UI Improvements
- **Inventory Bar Borders** - Added left and right borders to the bottom inventory display
  - Completes the bordered frame around the owned upgrades section
  - Matches the design consistency of other UI panels

---

## Previous Updates - February 15, 2026

### New Features
- **Supply Chain Issues Event** - Rare negative event that disrupts gameplay
  - 3% spawn chance every 5 seconds for challenging gameplay
  - Lasts 15 seconds when triggered
  - **Production Impact**: Reduces all bits per second by 50%
  - **Purchase Lockdown**: Disables all buy/sell buttons and PC building
  - **Visual Transformation**: Complete red theme takeover
    - Background switches to error.gif
    - All UI borders, text, and elements turn red
    - Red pulsing overlay on screen
    - Large countdown timer shows time remaining
    - Warning messages in all shop sections
  - **Event Blocking**: Prevents dhahab and threadripper from spawning during crisis
  - **Shop Display**: Shows "⚠️ PURCHASES DISABLED" banners
  - **Build Button**: Changes to "⚠️ SUPPLY CHAIN ISSUES"

- **Splash Screen** - Added animated splash screen when starting the game
  - Displays PC.png logo with glowing effect
  - Cinematic zoom-in animation from 30% to 120% scale
  - Shows game title and loading text
  - Zooms and fades out after 2.5 seconds before starting game

---

## Previous Updates - February 12, 2026

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
