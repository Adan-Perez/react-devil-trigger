# Changelog

## 0.5.1 - 2025-04-14

### Fixes

- Fixed CSS import issues when using the module in other projects
- Resolved "Can't resolve './base.css'" error occurring with some bundlers
- Ensured proper handling of CSS imports in the build process

### Technical Improvements

- Enhanced Rollup configuration for correctly processing CSS
- Guaranteed compatibility with various bundlers (webpack, vite, parcel)
- Improved CSS asset generation with proper path resolution

## 0.5.0 - 2025-04-14

### New Features

- Enhanced `DevilProgressBar` component with advanced visual effects:
  - Added fluid energy effects for all variant styles
  - Implemented dynamic glow effects that move with progress
  - Added particle and energy wave animations for stylized variant
  - Added responsive pulse effects for royal variant

### Enhancements

- Completely redesigned progress bar animations:
  - Eliminated visual glitches in stylized and royal variants
  - Improved visual continuity during progress transitions
  - Enhanced theme-specific effects (e.g., Dante's fire effects, Vergil's precision aesthetics)
  - Added depth layers for more professional look and feel

### Technical Improvements

- Refactored CSS animation system for better performance:
  - Separated progress tracking from visual effects
  - Used proper layering techniques for overlaid animations
  - Implemented hardware-accelerated animations with transform properties
  - Optimized keyframes for smoother transitions

## 0.4.0 - 2025-04-12

### New Features

- Added size variants for the player:
  - Four sizes available: sm, md, lg, xl
  - Responsive scaling of all elements including controls and fonts
  - Size-specific spacing and proportions
- Added center positioning options:
  - New top-center and bottom-center positions
  - Special handling for centered minimized state

### Enhancements

- Improved contrast in all character themes for better accessibility:
  - Enhanced text contrast with shadow effects
  - Better visibility for controls and interactive elements
  - Optimized color schemes for better WCAG compliance
- Enhanced visual styling for Nico's theme with mechanical workshop aesthetics
- Improved center positioning with proper transform handling for minimized state
- Added special effects for each character's theme when hovering over controls

### Technical Improvements

- Refined CSS architecture for better positioning edge cases
- Enhanced TypeScript type definitions with better documentation
- Added support for combined CSS transforms while maintaining positioning
- Improved class structure for more maintainable theme system

## 0.3.0 - 2025-04-11

### New Features

- Added Devil May Cry character themes with unique visual styles:
  - Dante: Red with golden accents and fire effects
  - Vergil: Blue with precision and sharp aesthetics
  - Nero: Bright blue with red Devil Breaker energy
  - V: Purple with teal accents and poetic styling
  - Trish: Golden with electric purple highlights
  - Lady: Deep red with black accents
  - Nico: Orange/brown with mechanical aesthetics
  - Sparda: Dark red with golden legendary effects
- Implemented background customization options:
  - Custom background color support
  - Adjustable background opacity
  - Configurable backdrop blur
- Added accent color support for interactive elements and animations

### Enhancements

- Complete CSS architecture refactoring for better maintainability:
  - Modular structure with separate files for base styles, layouts, controls, animations
  - Individual theme files for each DMC character
  - Improved organization of CSS variables
- Enhanced visual feedback for interactive elements
- Improved contrast and accessibility for all themes
- Added special effects and animations unique to each character
- Better documentation for all customization options

### Technical Improvements

- CSS code splitting for better maintainability
- Improved theme system with CSS variables
- Better prop validation and documentation
- Enhanced color handling with RGB value calculations for opacity effects

## 0.2.0 - 2025-04-08

### Enhancements

- Changed default value of `triggerWord` to `null`, preventing accidental activation during normal typing
- Improved volume control popup behavior with automatic closing:
  - Closes when clicking outside the popup
  - Closes when pressing the ESC key
  - Automatically closes when mouse is outside the area for 2 seconds
- Properly cleaned up timers and event listeners to prevent memory leaks

### Fixes

- Eliminated duplication of `AudioDevilTriggerProps` interface by using a single source of truth in `types/index.ts`

## 0.1.0 - 2025-04-07

- Initial release of React Devil Trigger module
- Customizable React audio player component
- Keyboard sequence detection for Easter eggs and hidden features
- TypeScript support and type definitions
- Rollup-based build system for optimized distribution
