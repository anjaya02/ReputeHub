# � UI Design System - Wireframe Specifications

**Reputify Reputation Management Platform**

> **Document Purpose:** Detailed wireframes for all pages with exact measurements, purple theme color annotations, spacing guidelines, and responsive breakpoint specifications.
>
> **For:** UI/UX Designers & Frontend Developers  
> **Last Updated:** November 2025  
> **Part of:** Reputify UI Design System Documentation

---

## Page-by-Page Layout Specifications

---

## � PURPLE THEME COLOR ANNOTATIONS

**Use these color codes when creating wireframes:**

### Primary Purple Colors

- **#720e9e** - Deep Purple (Headers, Hero sections)
- **#8b5cf6** - Royal Purple (Primary buttons, active states, accent text)
- **#a855f7** - Medium Purple (Interactive hover states)
- **#c084fc** - Light Purple (Hover borders, highlights)
- **#ddd6fe** - Pale Purple (Subtle borders)

### Background Colors

**Light Mode:**

- **#ffffff** - Main background
- **#faf5ff** - Sidebar, secondary areas (purple tint)
- **#f3e8ff** - Selected/hover backgrounds

**Dark Mode:**

- **#0f0f1e** - Main background (dark purple-tinted)
- **#1a1a2e** - Sidebar, cards (dark purple-gray)
- **#252542** - Hover states

### Interactive Elements

- **Buttons (Primary):** Purple gradient (#8b5cf6 → #a855f7)
- **Buttons (Secondary):** BG #e9d5ff with purple text
- **Links:** #8b5cf6 (royal purple)
- **Focus Ring:** 2px #8b5cf6 outline

### Semantic Colors

- **Success/Positive:** #22c55e (green)
- **Error/Negative:** #ef4444 (red)
- **Warning/Neutral:** #fb923c (amber)
- **Info:** #60a5fa (blue)

### Text Colors

**Light Mode:**

- Primary: #111827, Secondary: #4b5563, Tertiary: #9ca3af

**Dark Mode:**

- Primary: #f3f4f6, Secondary: #d1d5db, Tertiary: #9ca3af

### Wireframe Color Notation

When annotating wireframes, use:

- `[PURPLE-GRADIENT]` for hero elements
- `[PURPLE-BG]` for purple tinted backgrounds
- `[ROYAL-PURPLE]` for accent elements
- `[LIGHT-PURPLE]` for hover states

---

## �🏠 DASHBOARD PAGE WIREFRAME

### Desktop Layout (1440px) - Purple Theme Annotated

```
┌────────────────────────────────────────────────────────────────┐
│ HEADER BAR (Height: 64px)                                      │
│ BG: #ffffff (light) / #1a1a2e (dark)                           │
│ ┌──────┬─────────────────────────────────┬──────────────────┐ │
│ │ Logo │  Reputify Dashboard             │ 🔔 3  👤 John Doe │ │
│ │      │  [ROYAL-PURPLE text]            │ [PURPLE on hover] │ │
│ └──────┴─────────────────────────────────┴──────────────────┘ │
├────────────┬───────────────────────────────────────────────────┤
│ SIDEBAR    │ PAGE CONTENT (Padding: 32px)                      │
│ (W: 280px) │ BG: #ffffff (light) / #0f0f1e (dark)              │
│ BG: #faf5ff│ ┌─────────────────────────────────────────────┐  │
│ (light) or │ │ Welcome back, John! Here's your overview    │  │
│ #1a1a2e    │ └─────────────────────────────────────────────┘  │
│ (dark)     │                                                   │
│ ┌────────┐ │ KPI CARDS ROW (Grid: 4 columns, Gap: 24px)      │
│ │Dashboard│ │ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐│
│ │ ● Active│ │ │   87    │ │  0.72   │ │  156    │ │  3:1    ││
│ │[PURPLE- │ │ │ Rep.    │ │Sentiment│ │Mentions │ │Pos:Neg  ││
│ │GRADIENT]│ │ │ Index   │ │  Score  │ │This Week│ │ Ratio   ││
│ ├────────┤ │ │ ↑ 15%   │ │ ↑ 8%    │ │ ↓ 5%    │ │ → Same  ││
│ │Mentions │ │ └─────────┘ └─────────┘ └─────────┘ └─────────┘│
│ │[Gray    │ │ [PURPLE-    [White BG]  [White BG]  [White BG] │
│ │ text]   │ │ GRADIENT    Number in   Number in   Number in  │
│ ├────────┤ │ BG, White   ROYAL-      ROYAL-      ROYAL-      │
│ │ Alerts  │ │ text]       PURPLE]     PURPLE]     PURPLE]     │
│ │  (3)    │ │                                                   │
│ │[PURPLE  │ │ CHARTS SECTION (Grid: 2 columns, Gap: 32px)      │
│ │ badge]  │ │ ┌───────────────────┐ ┌───────────────────┐    │
│ ├────────┤ │ │SENTIMENT TREND    │ │PLATFORM BREAKDOWN │    │
│ │Reports  │ │ │Green/Red/Amber    │ │Purple gradient    │    │
│ │[Hover:  │ │ │   ╱╲    ╱╲       │ │slices             │    │
│ │#f3e8ff] │ │ │  ╱  ╲  ╱  ╲      │ │    ╱─────╲       │    │
│ ├────────┤ │ │ ╱    ╲╱    ╲     │ │   │   ●   │       │    │
│ │Integr.  │ │ │╱            ╲    │ │    ╲─────╱       │    │
│ │         │ │ │ Last 7 days      │ │    Google 30%     │    │
│ ├────────┤ │ └───────────────────┘ └───────────────────┘    │
│ │Settings │ │                                                   │
│ └────────┘ │ RECENT MENTIONS (Full width)                      │
│            │ ┌─────────────────────────────────────────────┐  │
│            │ │ Latest Activity          View All → [PURPLE]│  │
│            │ ├─────────────────────────────────────────────┤  │
│            │ │ [G] "Great service!" - 2h ago     😊 Positive│  │
│            │ │ [F] "Delivery was late" - 5h ago  😔 Negative│  │
│            │ │ [I] "Love the new menu!" - 1d ago 😊 Positive│  │
│            │ │ Hover: Border #c084fc (light purple)         │  │
│            │ └─────────────────────────────────────────────┘  │
└────────────┴───────────────────────────────────────────────────┘
```

### Mobile Layout (375px)

```
┌─────────────────┐
│ ☰  Dashboard  🔔 │ Header (56px)
├─────────────────┤
│ Welcome, John!  │
├─────────────────┤
│ ┌─────────────┐ │
│ │ 87 ↑15%     │ │ KPI Cards
│ │ Rep. Index  │ │ (Stack vertically)
│ └─────────────┘ │
│ ┌─────────────┐ │
│ │ 0.72 ↑8%    │ │
│ │ Sentiment   │ │
│ └─────────────┘ │
├─────────────────┤
│ SENTIMENT TREND │ Charts
│ [Line Chart]    │ (Full width)
├─────────────────┤
│ PLATFORMS       │
│ [Pie Chart]     │
├─────────────────┤
│ Recent Activity │ Mentions
│ • Great service │ (Compact cards)
│ • Delivery late │
├─────────────────┤
│ [Nav Bar]       │ Bottom Navigation
└─────────────────┘
```

---

## 📋 MENTIONS FEED WIREFRAME

### Desktop Layout

```
┌────────────────────────────────────────────────────────────────┐
│ MENTIONS FEED                                    Export ⬇️      │
├────────────────────────────────────────────────────────────────┤
│ FILTER BAR (Height: 80px, Background: Gray-50)                 │
│ ┌──────────┬──────────┬──────────┬──────────┬────────────┐   │
│ │Platform ▼│Sentiment▼│ Intent ▼ │Date Range│ 🔍 Search   │   │
│ └──────────┴──────────┴──────────┴──────────┴────────────┘   │
│                                        [Apply] [Clear]         │
├────────────────────────────────────────────────────────────────┤
│ Showing 156 mentions                           Sort: Newest ▼  │
├────────────────────────────────────────────────────────────────┤
│ MENTIONS LIST (Grid: 1 column, Gap: 16px)                      │
│ ┌──────────────────────────────────────────────────────────┐  │
│ │ [G] Google Reviews · 2 hours ago · API Badge              │  │
│ │ "The food was absolutely delicious and the service..."    │  │
│ │ 😊 Positive · Intent: Praise · ⭐⭐⭐⭐⭐                    │  │
│ │                                         [View Details →]  │  │
│ └──────────────────────────────────────────────────────────┘  │
│ ┌──────────────────────────────────────────────────────────┐  │
│ │ [F] Facebook · 5 hours ago · Apify Badge                  │  │
│ │ "Waited over an hour for delivery, very disappointed..."  │  │
│ │ 😔 Negative · Intent: Complaint · Cost: Paid              │  │
│ │                                         [View Details →]  │  │
│ └──────────────────────────────────────────────────────────┘  │
│                                                                │
│                    [Load More Mentions]                        │
└────────────────────────────────────────────────────────────────┘
```

---

## 🔍 MENTION DETAILS WIREFRAME

### Desktop Layout

```
┌────────────────────────────────────────────────────────────────┐
│ ← Back to Mentions        Mention Details         Actions ⚙️   │
├────────────────────────────────────────────────────────────────┤
│ MAIN CONTENT (70%)                    │ SIDEBAR (30%)         │
│ ┌──────────────────────────────────┐  │ ┌─────────────────┐  │
│ │ ORIGINAL POST                    │  │ │ QUICK ACTIONS   │  │
│ │ Platform: Facebook               │  │ │ [Respond]       │  │
│ │ Author: Jane Smith               │  │ │ [Flag]          │  │
│ │ Time: Oct 19, 2025 2:30 PM      │  │ │ [Archive]       │  │
│ │ ─────────────────────────────── │  │ └─────────────────┘  │
│ │ "I visited your restaurant last  │  │                       │
│ │ night and while the food was     │  │ ┌─────────────────┐  │
│ │ excellent, I was disappointed    │  │ │ AI INSIGHTS     │  │
│ │ with the service. We waited..."  │  │ │ Confidence: 94% │  │
│ │                                  │  │ │ Language: EN    │  │
│ │ [View on Facebook →]             │  │ │ Verified: ✓     │  │
│ └──────────────────────────────────┘  │ └─────────────────┘  │
│                                        │                       │
│ ┌──────────────────────────────────┐  │ ┌─────────────────┐  │
│ │ SENTIMENT ANALYSIS               │  │ │ SIMILAR         │  │
│ │ Overall: Mixed (65% Positive)    │  │ │ MENTIONS        │  │
│ │ ████████████░░░░░░              │  │ │                 │  │
│ │                                  │  │ │ • "Service      │  │
│ │ Aspects Detected:                │  │ │   issue" - 2d   │  │
│ │ • Food: 😊 Positive (92%)        │  │ │                 │  │
│ │ • Service: 😔 Negative (78%)     │  │ │ • "Slow         │  │
│ │ • Ambiance: 😐 Neutral (50%)     │  │ │   service" - 5d │  │
│ └──────────────────────────────────┘  │ │                 │  │
│                                        │ │ [View All →]    │  │
│ ┌──────────────────────────────────┐  │ └─────────────────┘  │
│ │ AI SUGGESTED RESPONSE            │  │                       │
│ │ ┌────────────────────────────┐  │  │                       │
│ │ │ Hi Jane, Thank you for     │  │  │                       │
│ │ │ your feedback. We're glad  │  │  │                       │
│ │ │ you enjoyed the food! We   │  │  │                       │
│ │ │ apologize for the service  │  │  │                       │
│ │ │ delay and we're working... │  │  │                       │
│ │ └────────────────────────────┘  │  │                       │
│ │ [Edit] [Approve & Send] [New]   │  │                       │
│ └──────────────────────────────────┘  │                       │
└────────────────────────────────────────┴───────────────────────┘
```

---

## 🚨 ALERTS PAGE WIREFRAME

### Desktop Layout

```
┌────────────────────────────────────────────────────────────────┐
│ ALERTS & NOTIFICATIONS                   Mark All Read ✓       │
├────────────────────────────────────────────────────────────────┤
│ Filter: [All Types ▼] [Last 24 hours ▼]        3 Active Alerts│
├────────────────────────────────────────────────────────────────┤
│                                                                │
│ ┌──────────────────────────────────────────────────────────┐  │
│ │ ⚠️ CRITICAL                                 30 mins ago   │  │
│ │ Google Reviews - 1★ Review                                │  │
│ │ "Worst experience ever. Food was cold and..."             │  │
│ │ Sentiment: Negative | Intent: Complaint                   │  │
│ │ [View Mention] [Respond Now] [Dismiss]                    │  │
│ └──────────────────────────────────────────────────────────┘  │
│                                                                │
│ ┌──────────────────────────────────────────────────────────┐  │
│ │ 🔴 HIGH PRIORITY                              2 hours ago │  │
│ │ Facebook - Multiple Negative Mentions                     │  │
│ │ "3 negative mentions detected in the last hour"           │  │
│ │ Platforms affected: Facebook (2), Instagram (1)           │  │
│ │ [View All] [Analyze Pattern] [Dismiss]                    │  │
│ └──────────────────────────────────────────────────────────┘  │
│                                                                │
│ RESOLVED ALERTS (Grayed out)                                  │
│ ┌──────────────────────────────────────────────────────────┐  │
│ │ ✓ RESOLVED                                    Yesterday   │  │
│ │ Reddit - Question about opening hours                     │  │
│ │ Response sent and customer satisfied                      │  │
│ │ [View Thread]                                             │  │
│ └──────────────────────────────────────────────────────────┘  │
└────────────────────────────────────────────────────────────────┘
```

---

## 📊 REPORTS PAGE WIREFRAME

### Desktop Layout

```
┌────────────────────────────────────────────────────────────────┐
│ REPORTS & INSIGHTS                      [Export PDF] [Export CSV]│
├────────────────────────────────────────────────────────────────┤
│ Period: [Last 30 days ▼] Platform: [All ▼]          Refresh 🔄 │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│ EXECUTIVE SUMMARY BOX                                          │
│ ┌──────────────────────────────────────────────────────────┐  │
│ │ 📈 Your reputation improved by 15% this month             │  │
│ │ • Total Mentions: 487 (↑23% from last month)             │  │
│ │ • Average Sentiment: 72% positive                        │  │
│ │ • Response Rate: 89% within 24 hours                     │  │
│ │ • Most Active Platform: Facebook (45% of mentions)       │  │
│ └──────────────────────────────────────────────────────────┘  │
│                                                                │
│ CHARTS GRID (2x2)                                              │
│ ┌─────────────────────┐ ┌─────────────────────┐              │
│ │ SENTIMENT OVER TIME │ │ MENTIONS BY PLATFORM│              │
│ │ [Line Chart]        │ │ [Bar Chart]         │              │
│ └─────────────────────┘ └─────────────────────┘              │
│ ┌─────────────────────┐ ┌─────────────────────┐              │
│ │ TOP ISSUES          │ │ RESPONSE TIME       │              │
│ │ 1. Service (23)     │ │ Avg: 2.5 hours      │              │
│ │ 2. Delivery (18)    │ │ [Progress Chart]    │              │
│ │ 3. Pricing (12)     │ │                     │              │
│ └─────────────────────┘ └─────────────────────┘              │
└────────────────────────────────────────────────────────────────┘
```

---

## 🔗 INTEGRATIONS PAGE WIREFRAME

### Desktop Layout

```
┌────────────────────────────────────────────────────────────────┐
│ PLATFORM INTEGRATIONS            Connected: 4/9    Add New +   │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│ CONNECTED PLATFORMS                                            │
│ ┌───────────────┐ ┌───────────────┐ ┌───────────────┐        │
│ │ [G] Google    │ │ [F] Facebook  │ │ [Y] YouTube   │        │
│ │ ● Connected   │ │ ● Connected   │ │ ● Connected   │        │
│ │ Reviews: 234  │ │ Posts: 156    │ │ Comments: 89  │        │
│ │ API (Free)    │ │ Graph API     │ │ API (Free)    │        │
│ │ [Settings]    │ │ [Settings]    │ │ [Settings]    │        │
│ └───────────────┘ └───────────────┘ └───────────────┘        │
│                                                                │
│ AVAILABLE PLATFORMS                                            │
│ ┌───────────────┐ ┌───────────────┐ ┌───────────────┐        │
│ │ [I] Instagram │ │ [L] LinkedIn  │ │ [T] TikTok    │        │
│ │ ○ Not Connected│ │ ○ Not Connected│ │ ○ Not Connected│       │
│ │ Apify (Paid)  │ │ Apify (Paid)  │ │ Apify (Paid)  │        │
│ │ Professional+ │ │ Business Only │ │ Business Only │        │
│ │ [Connect]     │ │ [Connect]     │ │ [Connect]     │        │
│ └───────────────┘ └───────────────┘ └───────────────┘        │
│                                                                │
│ ℹ️ Data Collection Schedule                                    │
│ • Official APIs refresh every 15 minutes                      │
│ • Apify automation runs every 8 hours                         │
│ • Next sync: in 2 hours 15 minutes                           │
└────────────────────────────────────────────────────────────────┘
```

---

## ⚙️ SETTINGS PAGE WIREFRAME

### Desktop Layout

```
┌────────────────────────────────────────────────────────────────┐
│ SETTINGS                                                       │
├─────────────┬──────────────────────────────────────────────────┤
│ TABS        │ CONTENT AREA                                     │
│ ┌─────────┐ │ ┌──────────────────────────────────────────────┐│
│ │ Profile  │ │ │ PROFILE INFORMATION                          ││
│ │ • Active │ │ │                                              ││
│ ├─────────┤ │ │ Business Name                                ││
│ │ Password │ │ │ [Cafe Aroma                    ]             ││
│ ├─────────┤ │ │                                              ││
│ │ Notific. │ │ │ Email                                        ││
│ ├─────────┤ │ │ [owner@cafearoma.lk            ]             ││
│ │ Billing  │ │ │                                              ││
│ ├─────────┤ │ │ Phone                                        ││
│ │ Advanced │ │ │ [+94 77 123 4567               ]             ││
│ └─────────┘ │ │                                              ││
│             │ │ Language                                      ││
│             │ │ [English ▼]                                  ││
│             │ │                                              ││
│             │ │ Timezone                                      ││
│             │ │ [Asia/Colombo (GMT+5:30) ▼]                  ││
│             │ │                                              ││
│             │ │            [Cancel] [Save Changes]           ││
│             │ └──────────────────────────────────────────────┘│
└─────────────┴──────────────────────────────────────────────────┘
```

---

## 👨‍💼 ADMIN PANEL WIREFRAMES

### Admin Overview

```
┌────────────────────────────────────────────────────────────────┐
│ ADMIN DASHBOARD                          Last updated: 2:30 PM │
├────────────────────────────────────────────────────────────────┤
│ SYSTEM METRICS                                                 │
│ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐         │
│ │ 156      │ │ 12,456   │ │ 72%      │ │ 99.9%    │         │
│ │ Active   │ │ Mentions │ │ Avg      │ │ Uptime   │         │
│ │ Clients  │ │ Today    │ │ Sentiment│ │ This Mo. │         │
│ └──────────┘ └──────────┘ └──────────┘ └──────────┘         │
│                                                                │
│ ┌─────────────────────────┐ ┌──────────────────────┐         │
│ │ CLIENT GROWTH           │ │ API USAGE           │         │
│ │ [Line Chart]            │ │ [Bar Chart]         │         │
│ └─────────────────────────┘ └──────────────────────┘         │
└────────────────────────────────────────────────────────────────┘
```

---

## 📐 SPACING & MEASUREMENTS

### Grid System

- **Container Max Width:** 1440px (desktop)
- **Sidebar Width:** 280px (desktop), 240px (tablet)
- **Content Padding:** 32px (desktop), 24px (tablet), 16px (mobile)
- **Card Padding:** 24px (all sides)
- **Grid Gap:** 24px (desktop), 16px (mobile)

### Component Heights

- **Header:** 64px (desktop), 56px (mobile)
- **Filter Bar:** 80px
- **KPI Card:** 120px
- **Mention Card:** 140px
- **Button:** 40px (default), 48px (large)
- **Input Field:** 40px

### Font Sizes

- **Page Title:** 32px
- **Section Header:** 24px
- **Card Title:** 20px
- **Body Text:** 16px
- **Small Text:** 14px
- **Tiny Label:** 12px

---

## 🎨 VISUAL HIERARCHY

### Z-Index Layers

```
0    - Background
100  - Page Content
200  - Cards & Containers
300  - Dropdowns
400  - Fixed Headers
500  - Sidebars
600  - Modals
700  - Toasts
800  - Tooltips
```

### Shadow Depths

- **Card:** 0 2px 4px rgba(0,0,0,0.1)
- **Hover Card:** 0 4px 6px rgba(0,0,0,0.15)
- **Modal:** 0 20px 25px rgba(0,0,0,0.2)
- **Dropdown:** 0 10px 15px rgba(0,0,0,0.1)

---

## 🎨 PURPLE THEME APPLICATION SUMMARY

### Key Purple Theme Elements to Include in Wireframes

**1. Navigation & Headers**

- Sidebar: Purple tinted background (#faf5ff light / #1a1a2e dark)
- Active nav item: Purple gradient with white text
- Top bar: Option for purple gradient or minimal with purple accents

**2. Hero Elements**

- Reputation Index KPI: Purple gradient background (#720e9e → #a855f7)
- Primary CTAs: Purple gradient buttons
- Page headers: Deep purple text (#720e9e)

**3. Interactive States**

- Default borders: Gray (#e5e7eb)
- Hover borders: Light purple (#c084fc)
- Focus rings: Royal purple (#8b5cf6)
- Active selections: Purple background tints

**4. Cards & Surfaces**

- Regular cards: White/dark with subtle borders
- Hover effect: Purple border + shadow glow
- Selected state: Purple background tint (#f3e8ff light / #252542 dark)

**5. Charts & Visualizations**

- Pie/Bar charts: Purple gradient spectrum (#720e9e through #d8b4fe)
- Sentiment lines: Keep semantic colors (green/red/amber)
- Grid lines: Subtle gray

**6. Buttons & Links**

- Primary: Purple gradient
- Secondary: Light purple BG with purple text
- Ghost: Transparent with purple on hover
- Links: Royal purple (#8b5cf6)

**7. Badges & Tags**

- Platform badges: Keep original brand colors
- Status dots: Green (connected) / Gray (disconnected)
- Sentiment badges: Keep semantic colors (green/red/amber)
- Count badges: Purple background

**8. Forms**

- Default: White/dark with gray border
- Focus: Purple border with purple shadow ring
- Error: Red border and background tint

**Design Tool Note:**
In Figma, create color styles for:

- `Brand/Deep Purple` (#720e9e)
- `Brand/Royal Purple` (#8b5cf6)
- `Brand/Medium Purple` (#a855f7)
- `Brand/Light Purple` (#c084fc)
- `Brand/Pale Purple` (#ddd6fe)
- `BG/Purple Tint Light` (#faf5ff)
- `BG/Purple Tint Strong` (#f3e8ff)
- `Gradient/Primary` (linear: #8b5cf6 → #a855f7)

---

This wireframe guide provides:
✅ Exact layout specifications
✅ Component positioning
✅ Content hierarchy
✅ Responsive behaviors
✅ Spacing measurements
✅ Visual hierarchy rules
✅ Complete purple theme color annotations

Your UI team can now create pixel-perfect wireframes in Figma with accurate purple theme styling!
