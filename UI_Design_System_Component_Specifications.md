# 📦 UI Design System - Component Specifications

**Reputify Reputation Management Platform**

> **Document Purpose:** Complete component library specifications including design tokens, color system, typography, spacing, and detailed component anatomy with purple theme implementation.
>
> **For:** UI/UX Designers & Frontend Developers  
> **Last Updated:** November 2025  
> **Part of:** Reputify UI Design System Documentation

---

## Detailed Component Design System

---

## 📐 DESIGN TOKENS & FOUNDATIONS

### Color Palette - Purple Theme System

#### Core Purple Brand Colors

```scss
// Primary Purple Spectrum
$deep-purple: #720e9e; // Darkest - Headers, important CTAs
$royal-purple: #8b5cf6; // Primary brand color
$medium-purple: #a855f7; // Interactive elements
$light-purple: #c084fc; // Hover states, accents
$pale-purple: #ddd6fe; // Backgrounds, subtle tints

// Extended Purple Shades
$purple-950: #3b0764; // Nearly black purple
$purple-900: #581c87; // Very dark purple
$purple-800: #6b21a8;
$purple-700: #7e22ce;
$purple-600: #9333ea;
$purple-500: #a855f7; // Medium purple (main)
$purple-400: #c084fc;
$purple-300: #d8b4fe;
$purple-200: #e9d5ff;
$purple-100: #f3e8ff;
$purple-50: #faf5ff; // Faintest tint
```

#### Semantic Colors (Sentiment & Status)

```scss
// Success (Positive Sentiment)
$success-dark: #14532d;
$success-main: #16a34a;
$success-light: #22c55e;
$success-pale: #dcfce7;

// Error (Negative Sentiment)
$error-dark: #7f1d1d;
$error-main: #dc2626;
$error-light: #ef4444;
$error-pale: #fee2e2;

// Warning (Neutral/Mixed Sentiment)
$warning-dark: #78350f;
$warning-main: #ea580c;
$warning-light: #fb923c;
$warning-pale: #fed7aa;

// Info (Informational)
$info-dark: #1e3a8a;
$info-main: #2563eb;
$info-light: #60a5fa;
$info-pale: #dbeafe;
```

#### Platform Brand Colors

```scss
$google: #4285f4;
$facebook: #1877f2;
$instagram: #e4405f;
$linkedin: #0a66c2;
$youtube: #ff0000;
$reddit: #ff4500;
$tiktok: #000000;
```

#### Neutral Colors

```scss
$gray-50: #f9fafb;
$gray-100: #f3f4f6;
$gray-200: #e5e7eb;
$gray-300: #d1d5db;
$gray-400: #9ca3af;
$gray-500: #6b7280;
$gray-600: #4b5563;
$gray-700: #374151;
$gray-800: #1f2937;
$gray-900: #111827;
```

#### Light Mode Variables

```scss
:root {
  // Backgrounds
  --bg-primary: #ffffff;
  --bg-secondary: #faf5ff; // Purple tinted (purple-50)
  --bg-tertiary: #f3e8ff; // Stronger purple tint (purple-100)
  --bg-elevated: #ffffff;
  --bg-overlay: rgba(0, 0, 0, 0.5);

  // Text Colors
  --text-primary: #111827;
  --text-secondary: #4b5563;
  --text-tertiary: #9ca3af;
  --text-inverse: #ffffff;

  // Interactive Elements
  --button-primary: #8b5cf6; // Royal purple
  --button-primary-hover: #7e22ce;
  --button-secondary: #e9d5ff;
  --button-secondary-hover: #d8b4fe;

  // Borders
  --border-default: #e5e7eb;
  --border-purple: #d8b4fe;
  --border-focus: #8b5cf6;

  // Surfaces
  --surface-card: #ffffff;
  --surface-hover: #faf5ff;
  --surface-selected: #f3e8ff;
  --surface-purple: #ddd6fe;

  // Gradients
  --gradient-purple: linear-gradient(135deg, #8b5cf6 0%, #a855f7 100%);
  --gradient-hero: linear-gradient(180deg, #faf5ff 0%, #ffffff 100%);
  --gradient-card: linear-gradient(135deg, #f3e8ff 0%, #ffffff 100%);
}
```

#### Dark Mode Variables

```scss
[data-theme="dark"] {
  // Backgrounds
  --bg-primary: #0f0f1e; // Very dark purple-tinted
  --bg-secondary: #1a1a2e; // Dark purple-gray
  --bg-tertiary: #252542;
  --bg-elevated: #2a2a4e;
  --bg-overlay: rgba(0, 0, 0, 0.7);

  // Text Colors
  --text-primary: #f3f4f6;
  --text-secondary: #d1d5db;
  --text-tertiary: #9ca3af;
  --text-inverse: #111827;

  // Interactive Elements
  --button-primary: #a855f7; // Medium purple
  --button-primary-hover: #c084fc;
  --button-secondary: #3b0764;
  --button-secondary-hover: #581c87;

  // Borders
  --border-default: #374151;
  --border-purple: #6b21a8;
  --border-focus: #a855f7;

  // Surfaces
  --surface-card: #1a1a2e;
  --surface-hover: #252542;
  --surface-selected: #2a2a4e;
  --surface-purple: #3b0764;

  // Gradients
  --gradient-purple: linear-gradient(135deg, #720e9e 0%, #a855f7 100%);
  --gradient-hero: linear-gradient(180deg, #0f0f1e 0%, #1a1a2e 100%);
  --gradient-card: linear-gradient(135deg, #252542 0%, #1a1a2e 100%);
}
```

### Typography Scale

```scss
// Font Family
$font-primary: "Inter", -apple-system, sans-serif;
$font-mono: "JetBrains Mono", monospace;

// Font Sizes
$text-xs: 12px; // Tiny labels
$text-sm: 14px; // Small text
$text-base: 16px; // Body text
$text-lg: 18px; // Large body
$text-xl: 20px; // H3
$text-2xl: 24px; // H2
$text-3xl: 30px; // H1
$text-4xl: 36px; // Display

// Font Weights
$font-normal: 400;
$font-medium: 500;
$font-semibold: 600;
$font-bold: 700;

// Line Heights
$leading-tight: 1.25;
$leading-normal: 1.5;
$leading-relaxed: 1.75;
```

### Spacing System (8px Grid)

```scss
$space-0: 0px;
$space-1: 4px;
$space-2: 8px;
$space-3: 12px;
$space-4: 16px;
$space-5: 20px;
$space-6: 24px;
$space-8: 32px;
$space-10: 40px;
$space-12: 48px;
$space-16: 64px;
```

### Border Radius

```scss
$rounded-none: 0px;
$rounded-sm: 4px;
$rounded-md: 6px;
$rounded-lg: 8px;
$rounded-xl: 12px;
$rounded-2xl: 16px;
$rounded-full: 9999px;
```

### Shadows

```scss
$shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.05);
$shadow-md: 0 4px 6px rgba(0, 0, 0, 0.07);
$shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.1);
$shadow-xl: 0 20px 25px rgba(0, 0, 0, 0.1);
```

---

## 🧩 COMPONENT SPECIFICATIONS

### 1. KPI CARD Component

**Purpose:** Display key metrics with visual indicators

**Anatomy:**

```
┌─────────────────────────┐
│ Icon    Title      ↑15% │
│         Value            │
│         Subtitle         │
└─────────────────────────┘
```

**Properties:**

- `icon`: IconType (required)
- `title`: string (required)
- `value`: string | number (required)
- `subtitle`: string (optional)
- `trend`: number (optional)
- `trendDirection`: 'up' | 'down' | 'neutral'
- `loading`: boolean

**States:**

- Default
- Loading (skeleton)
- Hover (slight elevation)
- Error (red border)

**Variations:**

- Small (Dashboard widget)
- Large (Featured metric)
- Compact (Mobile)

**Usage Example:**

```jsx
<KPICard
  icon="TrendingUp"
  title="Reputation Index"
  value="87"
  subtitle="Out of 100"
  trend={15}
  trendDirection="up"
/>
```

---

### 2. MENTION CARD Component

**Purpose:** Preview of social media mention

**Anatomy:**

```
┌──────────────────────────────┐
│ [FB] 2 hours ago      [API]  │
│ ─────────────────────────────│
│ "The service was really..."   │
│                               │
│ 😊 Positive | Intent: Praise  │
│ ─────────────────────────────│
│ [View Details →]              │
└──────────────────────────────┘
```

**Properties:**

- `platform`: PlatformType (required)
- `timestamp`: Date (required)
- `text`: string (required, max 200 chars)
- `sentiment`: 'positive' | 'negative' | 'neutral'
- `intent`: 'complaint' | 'praise' | 'question' | 'request'
- `dataSource`: 'api' | 'apify'
- `isNew`: boolean
- `onClick`: function

**States:**

- Default
- Hover (shadow + cursor)
- Selected (border highlight)
- New (blue dot indicator)
- Loading

**Responsive:**

- Desktop: 3-column grid
- Tablet: 2-column grid
- Mobile: Single column

---

### 3. SENTIMENT BADGE Component

**Purpose:** Color-coded sentiment indicator

**Anatomy:**

```
[😊 Positive]  [😐 Neutral]  [😔 Negative]
```

**Properties:**

- `sentiment`: 'positive' | 'negative' | 'neutral' | 'mixed'
- `score`: number (0-1)
- `size`: 'sm' | 'md' | 'lg'
- `showIcon`: boolean
- `showScore`: boolean

**Color Mapping (Purple Theme):**

- Positive: Green (#22c55e / #16a34a)
  - Light mode: BG #dcfce7, Text #14532d
  - Dark mode: BG #14532d, Text #22c55e
- Negative: Red (#ef4444 / #dc2626)
  - Light mode: BG #fee2e2, Text #7f1d1d
  - Dark mode: BG #7f1d1d, Text #ef4444
- Neutral: Amber (#fb923c / #ea580c)
  - Light mode: BG #fed7aa, Text #78350f
  - Dark mode: BG #78350f, Text #fb923c
- Mixed: Gray (#6B7280)

**Variations:**

- Pill style (rounded-full)
- Square style (rounded-md)
- Minimal (text only)
- Detailed (icon + text + score)

---

### 4. PLATFORM BADGE Component

**Purpose:** Platform identification with status

**Anatomy:**

```
[G] Google  [F] Facebook  [I] Instagram
    ●           ●              ○
Connected   Connected    Disconnected
```

**Properties:**

- `platform`: PlatformType
- `status`: 'connected' | 'disconnected' | 'error'
- `showStatus`: boolean
- `size`: 'sm' | 'md' | 'lg'
- `method`: 'api' | 'apify'

**Visual Specs:**

- Icon: Platform brand color
- Status dot: Green/Red/Gray
- Background: Light gray
- Border: 1px solid border color

---

### 5. FILTER DROPDOWN Component

**Purpose:** Multi-select filtering control

**Anatomy:**

```
┌─────────────────────┐
│ Platform      ▼     │
├─────────────────────┤
│ ☐ All Platforms     │
│ ☑ Google Reviews    │
│ ☑ Facebook          │
│ ☐ Instagram         │
│ [Apply] [Clear]     │
└─────────────────────┘
```

**Properties:**

- `label`: string
- `options`: Array<{value, label, count}>
- `selected`: Array<string>
- `multiple`: boolean
- `showCount`: boolean
- `onChange`: function

**States:**

- Closed
- Open
- Filtered (shows count)
- Disabled

**Behavior:**

- Click outside to close
- Keyboard navigation
- Select all/none option
- Search within options

---

### 6. CHART COMPONENTS

#### Line Chart (Sentiment Trend)

```
100 ┤     ╭─╮
 75 ┤  ╭─╯  ╰─╮
 50 ┤─╯      ╰
 25 ┤
  0 └─────────────
    Mon  Wed  Fri
```

**Properties:**

- `data`: Array<{x, y}>
- `xAxis`: AxisConfig
- `yAxis`: AxisConfig
- `color`: string
- `showGrid`: boolean
- `showTooltip`: boolean
- `height`: number

#### Pie Chart (Platform Distribution)

```
     Facebook 45%
    ╱─────╲
   │   ●   │  Google 30%
    ╲─────╱
     Other 25%
```

**Properties:**

- `data`: Array<{label, value, color}>
- `showLegend`: boolean
- `showPercentage`: boolean
- `donut`: boolean
- `size`: number

---

### 7. ALERT CARD Component

**Purpose:** High-priority notification display

**Anatomy:**

```
┌──────────────────────────────┐
│ ⚠️ CRITICAL ALERT             │
│ ─────────────────────────────│
│ Platform: Google Reviews      │
│ "Worst experience ever..."    │
│ Severity: ████░ High          │
│ ─────────────────────────────│
│ [View] [Respond] [Dismiss]    │
└──────────────────────────────┘
```

**Properties:**

- `severity`: 'low' | 'medium' | 'high' | 'critical'
- `platform`: PlatformType
- `message`: string
- `timestamp`: Date
- `actions`: Array<Action>

**Color Coding:**

- Critical: Red background
- High: Orange background
- Medium: Yellow background
- Low: Blue background

---

### 8. EMPTY STATE Component

**Purpose:** Placeholder when no data exists

**Anatomy:**

```
┌──────────────────────────────┐
│                              │
│         [Illustration]        │
│                              │
│    No mentions found yet     │
│   Connect a platform to      │
│     start monitoring         │
│                              │
│    [Connect Platform]        │
└──────────────────────────────┘
```

**Properties:**

- `icon`: IconType
- `title`: string
- `description`: string
- `action`: {label, onClick}
- `illustration`: ImageUrl

**Variations:**

- No data
- No results (search/filter)
- Error occurred
- Coming soon

---

### 9. LOADING SKELETON Component

**Purpose:** Placeholder during data loading

**Types:**

```
Text Skeleton:
████████████████ 100%
████████ 40%

Card Skeleton:
┌──────────────┐
│ ████  ██████ │
│ ████████████ │
│ ████████     │
└──────────────┘
```

**Properties:**

- `type`: 'text' | 'card' | 'chart' | 'table'
- `lines`: number
- `height`: number
- `animate`: boolean

---

### 10. MODAL Component

**Purpose:** Overlay dialogs for actions

**Anatomy:**

```
┌─────────────────────────────┐
│ Modal Title            [X]   │
│ ─────────────────────────── │
│                             │
│ Modal content goes here...   │
│                             │
│ ─────────────────────────── │
│        [Cancel] [Confirm]    │
└─────────────────────────────┘
```

**Properties:**

- `isOpen`: boolean
- `title`: string
- `size`: 'sm' | 'md' | 'lg' | 'xl'
- `closeOnOverlay`: boolean
- `showCloseButton`: boolean
- `footer`: ReactNode

**Behavior:**

- Trap focus
- ESC to close
- Overlay click to close
- Smooth animations

---

### 11. TOAST NOTIFICATION Component

**Purpose:** Temporary feedback messages

**Anatomy:**

```
┌─────────────────────┐
│ ✅ Success!     [X] │
│ Reply sent          │
└─────────────────────┘
```

**Properties:**

- `type`: 'success' | 'error' | 'info' | 'warning'
- `title`: string
- `message`: string
- `duration`: number (ms)
- `position`: 'top-right' | 'bottom-center' etc

**Auto-dismiss timing:**

- Success: 3 seconds
- Info: 4 seconds
- Warning: 5 seconds
- Error: No auto-dismiss

---

## 📱 RESPONSIVE COMPONENT BEHAVIORS

### Mobile Adaptations

**Navigation:**

- Sidebar → Bottom navigation
- Breadcrumb → Back button
- Tabs → Horizontal scroll

**Cards:**

- Multi-column → Single column
- Horizontal cards → Vertical stack
- Reduced padding (24px → 16px)

**Tables:**

- Full table → Card list
- Hidden columns → Expandable rows
- Horizontal scroll for wide tables

**Modals:**

- Centered → Full screen
- Multiple buttons → Stacked buttons
- Large forms → Step-by-step

**Charts:**

- Interactive → Static images
- Detailed → Simplified
- Tooltips → Tap to show

---

## 🎭 COMPONENT STATES

### Interactive States

```
Default → Hover → Active → Focus → Disabled
```

### Loading States

```
Initial → Loading → Success/Error → Retry
```

### Form States

```
Empty → Focused → Filled → Valid → Invalid → Submitted
```

---

## ♿ ACCESSIBILITY REQUIREMENTS

### All Components Must Have:

- Keyboard navigation support
- ARIA labels and roles
- Focus indicators
- Screen reader descriptions
- Color contrast (WCAG AA)
- Touch target size (44x44px minimum)

### Specific Requirements:

- **Modals:** Focus trap, ESC to close
- **Dropdowns:** Arrow key navigation
- **Charts:** Alternative text descriptions
- **Forms:** Error announcements
- **Toasts:** ARIA live regions

---

## 🎨 DARK MODE SPECIFICATIONS

### Color Inversions:

- Backgrounds: Light → Dark
- Text: Dark → Light
- Borders: Subtle adjustment
- Shadows: Reduced opacity

### Component Adjustments:

- Cards: Dark gray background
- Input fields: Dark with light text
- Charts: Adjusted color palette
- Platform badges: Maintained brand colors

---

## 🎨 PURPLE THEME COMPONENT STYLING

### Button Implementations

```scss
// Primary Button
.btn-primary {
  background: var(--gradient-purple);
  color: white;

  &:hover {
    background: linear-gradient(135deg, #6b21a8 0%, #9333ea 100%);
    box-shadow: 0 4px 12px rgba(139, 92, 246, 0.3);
  }
}

// Secondary Button
.btn-secondary {
  background: var(--button-secondary);
  color: var(--royal-purple);
  border: 1px solid var(--border-purple);

  &:hover {
    background: var(--button-secondary-hover);
  }
}

// Ghost Button
.btn-ghost {
  background: transparent;
  color: var(--royal-purple);

  &:hover {
    background: var(--surface-hover);
  }
}
```

### KPI Card Styling

```scss
// Hero Card (Reputation Index)
.kpi-hero {
  background: var(--gradient-purple);
  color: white;

  .kpi-value {
    font-size: 48px;
    font-weight: 700;
  }

  .kpi-trend {
    color: rgba(255, 255, 255, 0.9);
  }
}

// Regular KPI Cards
.kpi-card {
  background: var(--surface-card);
  border: 1px solid var(--border-default);

  &:hover {
    border-color: var(--border-purple);
    box-shadow: 0 0 0 3px rgba(139, 92, 246, 0.1);
    transform: translateY(-2px);
  }

  .kpi-value {
    color: var(--royal-purple);
  }
}
```

### Mention Card Styling

```scss
.mention-card {
  background: var(--surface-card);
  border: 1px solid var(--border-default);
  border-radius: 8px;

  &:hover {
    border-color: var(--light-purple);
    box-shadow: 0 10px 20px rgba(139, 92, 246, 0.1);
  }

  &.highlight {
    border-color: var(--royal-purple);
    box-shadow: 0 0 0 3px rgba(139, 92, 246, 0.1);
  }
}
```

### Navigation Sidebar Styling

```scss
.sidebar {
  background: var(--bg-secondary);

  .nav-item {
    color: var(--text-secondary);

    &.active {
      background: var(--gradient-purple);
      color: white;
      border-radius: 8px;
    }

    &:hover {
      background: var(--surface-hover);
      color: var(--royal-purple);
    }
  }
}
```

### Alert Card Styling

```scss
.alert-critical {
  background: var(--error-pale);
  border-left: 4px solid var(--error-main);

  [data-theme="dark"] & {
    background: var(--error-dark);
    border-color: var(--error-light);
  }
}

.alert-high {
  background: var(--warning-pale);
  border-left: 4px solid var(--warning-main);

  [data-theme="dark"] & {
    background: var(--warning-dark);
    border-color: var(--warning-light);
  }
}
```

### Chart Color Schemes

```scss
// Sentiment Trend (Line Chart)
.chart-sentiment {
  --line-positive: #22c55e;
  --line-negative: #ef4444;
  --line-neutral: #fb923c;
  --grid-lines: var(--border-default);
}

// Platform Distribution (Pie Chart)
.chart-platform {
  --slice-1: #720e9e; // Deep purple
  --slice-2: #8b5cf6; // Royal purple
  --slice-3: #a855f7; // Medium purple
  --slice-4: #c084fc; // Light purple
  --slice-5: #d8b4fe; // Pale purple
}

// Mention Volume (Bar Chart)
.chart-volume {
  --bar-primary: var(--gradient-purple);
  --bar-comparison: var(--surface-selected);
}
```

### Form Input Styling

```scss
.input-field {
  background: var(--bg-primary);
  border: 1px solid var(--border-default);
  color: var(--text-primary);

  &:focus {
    border-color: var(--border-focus);
    box-shadow: 0 0 0 3px rgba(139, 92, 246, 0.1);
    outline: none;
  }

  &.error {
    border-color: var(--error-main);
    background: var(--error-pale);
  }
}
```

### Special Effects

```scss
// Glassmorphism (Premium features)
.glass-card {
  background: rgba(139, 92, 246, 0.1);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(139, 92, 246, 0.2);
}

// Glow Effect
.glow-purple {
  box-shadow: 0 0 20px rgba(139, 92, 246, 0.3), 0 0 40px rgba(139, 92, 246, 0.2),
    0 0 60px rgba(139, 92, 246, 0.1);
}

// Loading Shimmer
.shimmer {
  background: linear-gradient(
    90deg,
    var(--surface-card) 0%,
    var(--pale-purple) 50%,
    var(--surface-card) 100%
  );
  background-size: 200% 100%;
  animation: shimmer 2s infinite;
}

@keyframes shimmer {
  0% {
    background-position: 100% 0;
  }
  100% {
    background-position: -100% 0;
  }
}
```

### Accessibility Considerations

```scss
// WCAG AAA Compliant combinations
// Purple on white: #720e9e on #ffffff = 7.5:1 ✅
// White on purple: #ffffff on #8b5cf6 = 4.5:1 ✅

:focus-visible {
  outline: 2px solid var(--royal-purple);
  outline-offset: 2px;
}

// High contrast mode
@media (prefers-contrast: high) {
  :root {
    --royal-purple: #6b21a8; // Darker for better contrast
  }
}

// Reduced motion
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    transition-duration: 0.01ms !important;
  }
}
```

---

## 📦 COMPONENT EXPORT STRUCTURE

```
/components
  /atoms
    - Button
    - Badge
    - Icon
    - Input
  /molecules
    - KPICard
    - MentionCard
    - PlatformBadge
    - FilterDropdown
  /organisms
    - NavigationSidebar
    - MentionsList
    - DashboardGrid
    - AlertsPanel
  /templates
    - PageLayout
    - AuthLayout
    - AdminLayout
```

---

This component specification document provides:
✅ Complete design tokens
✅ Detailed component anatomy
✅ All properties and states
✅ Responsive behaviors
✅ Accessibility requirements
✅ Implementation guidelines

Your UI team can now build a consistent, scalable component library!
