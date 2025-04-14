# React Devil Trigger

<p align="center">
  <img 
    src="./images/logo-letters.webp" 
    alt="React Devil Trigger Logo" 
    width="400" 
    style="filter: drop-shadow(0 0 8px rgba(255, 0, 0, 0.8)) drop-shadow(0 0 20px rgba(255, 0, 0, 0.4));" 
  />
</p>

[![npm version](https://img.shields.io/npm/v/react-devil-trigger.svg)](https://www.npmjs.com/package/react-devil-trigger)
[![npm downloads](https://img.shields.io/npm/dm/react-devil-trigger.svg)](https://www.npmjs.com/package/react-devil-trigger)
[![License](https://img.shields.io/npm/l/react-devil-trigger.svg)](https://github.com/Adan-Perez/react-devil-trigger/blob/main/LICENSE)
[![Bundle Size](https://img.shields.io/bundlephobia/minzip/react-devil-trigger)](https://bundlephobia.com/package/react-devil-trigger)

A stylish collection of React components with dynamic features and special effects, inspired by the fast-paced action of Devil May Cry.

## 🆕 What's New in v0.5.0

- **Enhanced Progress Bars**: Fluid animations and energy effects for all progress bar variants
- **Improved Visual Effects**: Dynamic glow effects, particle animations, and depth layers
- **Technical Improvements**: Better performance and smoother animations

## Installation

```bash
npm install react-devil-trigger
```

> [!IMPORTANT]
> You need to import the CSS styles in your main file (e.g., `main.tsx` or `App.jsx`) to apply the default styles and animations.

```javascript
import 'react-devil-trigger/dist/devil-trigger.css'; // Import CSS styles in your main file
```

## Components

### AudioDevilTrigger

Stylish audio player with Devil May Cry themes and effects.

```jsx
import { AudioDevilTrigger } from 'react-devil-trigger';

function App() {
  return (
    <div>
      <AudioDevilTrigger
        audioSrc='path-to-audio.mp3'
        triggerKey='jackpot' // Optional trigger word
        characterTheme='dante'
      />
    </div>
  );
}
```

### DevilProgressBar

Dynamic progress bars with Devil May Cry inspired effects and animations.

```jsx
import { DevilProgressBar } from 'react-devil-trigger';

function App() {
  const [progress, setProgress] = useState(50);

  return (
    <div>
      <DevilProgressBar
        progress={progress}
        variant='stylized'
        characterTheme='dante'
        label='Devil Trigger'
        showPercentage={true}
      />
    </div>
  );
}
```

## Progress Bar Variants

Choose from various stylistic variants:

```jsx
// Default style
<DevilProgressBar progress={75} />

// Stylized with energy effects
<DevilProgressBar progress={75} variant="stylized" />

// Devil Trigger gauge
<DevilProgressBar progress={75} variant="dt" />

// Sin Devil Trigger gauge (more intense effects)
<DevilProgressBar progress={75} variant="sdt" />

// Royal Guard style
<DevilProgressBar progress={75} variant="royal" />
```

## Progress Bar Sizes

Choose from different size options:

```jsx
<DevilProgressBar progress={75} height="xs" />
<DevilProgressBar progress={75} height="sm" />
<DevilProgressBar progress={75} height="md" /> // Default
<DevilProgressBar progress={75} height="lg" />
<DevilProgressBar progress={75} height="xl" />
```

## Character Themes

Choose from various Devil May Cry character themes:

```jsx
<AudioDevilTrigger
  audioSrc="devils-never-cry.mp3"
  characterTheme="dante"
/>

<DevilProgressBar
  progress={75}
  characterTheme="vergil"
  variant="sdt"
/>
```

Available themes: `dante`, `vergil`, `nero`, `v`, `trish`, `lady`, `nico`, `sparda`, `default`

## Positioning Options

Choose where the player appears on the screen:

```jsx
<AudioDevilTrigger
  position="bottom-right" // Default position
/>

<AudioDevilTrigger
  position="top-center" // Centered at the top
/>

<AudioDevilTrigger
  position="bottom-center" // Centered at the bottom
/>
```

Available positions: `bottom-right`, `bottom-left`, `top-right`, `top-left`, `bottom-center`, `top-center`

## Size Variants

Choose the size that fits your design:

```jsx
<AudioDevilTrigger
  size="sm" // Small size
/>

<AudioDevilTrigger
  size="lg" // Large size
/>
```

Available sizes: `sm`, `md` (default), `lg`, `xl`

## Customizing Background

When customizing the background, there are two ways to set opacity:

1. **Using `backgroundColor` with opacity included**:

```jsx
<AudioDevilTrigger
  backgroundColor='rgba(0, 0, 0, 0.7)'
  // backgroundOpacity is ignored when using rgba/hsla format
/>
```

2. **Using `backgroundColor` with `backgroundOpacity`**:

```jsx
<AudioDevilTrigger
  backgroundColor='#000000' // or any color name or hex code
  backgroundOpacity={0.7} // This will be applied to the color
/>
```

You can also adjust the backdrop blur effect:

```jsx
<AudioDevilTrigger
  backdropBlur={5} // Custom blur value in pixels
  // or
  backdropBlur={false} // Disable blur
/>
```

## Color Customization

Each theme comes with predefined colors, but you can override them:

```jsx
<AudioDevilTrigger
  characterTheme='vergil'
  primaryColor='#0055aa' // Override primary color
  secondaryColor='#ffffff' // Override secondary color
  accentColor='#00ffee' // Override accent color
/>
```

## Documentation

- [CHANGELOG](./CHANGELOG.md) - History of changes (English)
- [CHANGELOG en Español](./CHANGELOG.es.md) - Historial de cambios (Español)

## Developers

| Author     | GitHub                                      |
| ---------- | ------------------------------------------- |
| Adan-Perez | [Adan-Perez](https://github.com/Adan-Perez) |

## License

ISC License - see [LICENSE](LICENSE) for details

<p align="left">
  <img src="./images/logo.webp" alt="React Devil Trigger Logo" width="150" />
</p>
