# 🗺️ UI Design System - Complete Roadmap

**Reputify Reputation Management Platform**

> **Document Purpose:** Comprehensive page-by-page design roadmap covering all 55+ screens, component requirements, purple theme visual identity, and implementation priorities.
>
> **For:** UI/UX Designers & Project Managers  
> **Last Updated:** November 2025  
> **Part of:** Reputify UI Design System Documentation

---

## Complete Frontend Development Blueprint

---

## 📊 Overview Statistics

- **Total Unique Screens:** 55+ (including all states)
- **Client Portal Pages:** 11
- **Admin Panel Pages:** 5
- **Component Library Items:** 40+
- **Responsive Breakpoints:** 3 (Desktop, Tablet, Mobile)
- **Color Theme:** Purple Brand System

---

## 🎨 PURPLE THEME VISUAL IDENTITY

### Brand Color Application

Reputify uses a **purple-based color system** to create a modern, premium SaaS experience:

**Purple Usage Guidelines:**

- **Headers/Navigation:** Gradient purple backgrounds (#720e9e → #a855f7)
- **CTAs:** Purple gradient buttons for primary actions
- **Active States:** Royal purple (#8b5cf6) for selected items
- **Backgrounds:** Subtle purple tints (#faf5ff) for depth
- **Hover Effects:** Light purple (#c084fc) for interactivity
- **Borders:** Pale purple (#ddd6fe) for subtle separation

**Visual Examples:**

```
NAVIGATION SIDEBAR:
Light Mode: BG #faf5ff (purple tint)
Active Item: Purple gradient with white text
Hover: BG #f3e8ff

HERO KPI CARD (Reputation Index):
Background: Purple gradient (#720e9e → #a855f7)
Text: White with high contrast

REGULAR KPI CARDS:
Background: White / Dark (#1a1a2e)
Value Number: Royal purple (#8b5cf6)
Hover Border: Light purple (#c084fc)

BUTTONS:
Primary: Purple gradient
Secondary: Light purple BG (#e9d5ff) with purple text
Ghost: Transparent with purple text, purple BG on hover

MENTION CARDS:
Background: White / Dark
Border: Gray (default) → Light purple on hover
Highlight: Purple border with purple shadow glow
```

**Platform Colors Preserved:**

- Google: #4285F4 (blue)
- Facebook: #1877F2 (blue)
- Instagram: #E4405F (pink-red)
- LinkedIn: #0A66C2 (blue)
- Keep these unchanged for brand recognition

**Sentiment Colors:**

- Positive: Green (#22c55e)
- Negative: Red (#ef4444)
- Neutral: Amber (#fb923c)
- Keep these for clear emotional signaling

---

## 🗺️ NAVIGATION ARCHITECTURE

### Primary Navigation Structure

```
Reputify
├── 🌐 Public Area (No Auth)
│   ├── Landing Page
│   ├── Login Page
│   └── Signup Page
│
├── 👤 Client Portal (Auth Required)
│   ├── Dashboard (Home)
│   ├── Mentions Feed
│   │   └── Mention Details (sub-page)
│   ├── Alerts
│   ├── Reports & Insights
│   ├── Integrations
│   └── Settings
│
└── 👨‍💼 Admin Panel (Admin Auth)
    ├── Admin Overview
    ├── Manage Clients
    ├── Monitor Jobs
    ├── Billing & Plans
    └── System Logs
```

---

## 🎯 SCREEN-BY-SCREEN SPECIFICATION

### 🌍 PUBLIC AREA (3 Screens)

#### 1. **LANDING PAGE**

**Purpose:** Marketing & conversion
**URL:** `/`

**Sections to Design:**

```
┌─────────────────────────────────────┐
│ HEADER                              │
│ • Logo (left)                       │
│ • Nav: Features|Pricing|About|Contact│
│ • CTA: Login | Sign Up (right)      │
├─────────────────────────────────────┤
│ HERO SECTION                        │
│ • Headline: "Listen Smarter.        │
│   Respond Faster."                  │
│ • Subtext (value prop)              │
│ • CTA Button: "Start Free Trial"    │
│ • Hero Image/Animation              │
├─────────────────────────────────────┤
│ FEATURES OVERVIEW (4 Cards)         │
│ • Monitor • Analyze                 │
│ • Engage  • Improve                 │
├─────────────────────────────────────┤
│ PLATFORM SHOWCASE                   │
│ • 7 Platform Icons in grid          │
│ • (Google, FB, IG, LinkedIn,        │
│    TikTok, YouTube, Reddit)         │
├─────────────────────────────────────┤
│ PRICING TABLE                       │
│ • Starter (LKR 3,000)               │
│ • Professional (LKR 9,000)          │
│ • Business (LKR 24,000)             │
├─────────────────────────────────────┤
│ FOOTER                              │
│ • Contact: info@reputify.lk         │
│ • Phone: +94 711687980              │
│ • Links: Privacy|Terms|Support      │
└─────────────────────────────────────┘
```

#### 2. **LOGIN PAGE**

**Purpose:** User authentication
**URL:** `/login`

**Components:**

- Logo + "Reputify Portal" title
- Email input field
- Password input field
- "Remember me" checkbox
- "Forgot password?" link
- "Sign In" button (primary)
- Divider with "OR"
- "Continue with Google" button (optional)
- "New user? Create account" link
- Error message area

#### 3. **SIGNUP PAGE**

**Purpose:** New account creation
**URL:** `/signup`

**Components:**

- Logo + "Create Your Account" title
- Business Name input
- Email input
- Password input
- Confirm Password input
- Plan selection (radio buttons):
  - Starter
  - Professional
  - Business
- Terms checkbox
- "Create Account" button
- "Already have an account? Login" link
- Error/success message area

---

### 👤 CLIENT PORTAL (8 Main Screens + Sub-pages)

#### 4. **DASHBOARD (HOME)**

**Purpose:** Overview of reputation status
**URL:** `/dashboard`

**Layout Structure:**

```
┌─────────────────────────────────────┐
│ TOP BAR                             │
│ • Logo • User Menu • Notifications  │
├────┬────────────────────────────────┤
│    │ MAIN CONTENT AREA              │
│ S  ├────────────────────────────────┤
│ I  │ KPI CARDS ROW (4 cards)        │
│ D  │ • AI Reputation Index (0-100)  │
│ E  │ • Avg Sentiment Score          │
│ B  │ • Total Mentions (today/week)  │
│ A  │ • Positive vs Negative Ratio   │
│ R  ├────────────────────────────────┤
│    │ CHARTS ROW (2 columns)         │
│ M  │ • Sentiment Trend Graph        │
│ E  │ • Platform Breakdown Pie       │
│ N  ├────────────────────────────────┤
│ U  │ LATEST MENTIONS                │
│    │ • 3 Recent mention cards       │
│    │ • "View All" button            │
└────┴────────────────────────────────┘
```

**Sidebar Menu Items:**

- Dashboard (active)
- Mentions Feed
- Alerts
- Reports
- Integrations
- Settings
- Logout

#### 5. **MENTIONS FEED**

**Purpose:** View all collected mentions
**URL:** `/mentions`

**Top Section - Filters Bar:**

- Platform dropdown (All, Google, Facebook, Instagram, etc.)
- Data Source dropdown (Official API, Apify, All)
- Sentiment dropdown (Positive, Negative, Neutral, All)
- Intent dropdown (Complaint, Praise, Question, All)
- Date range picker
- Search input field
- "Apply Filters" button
- "Clear Filters" link

**Main Section - Mentions List:**

```
Each Mention Card Contains:
┌─────────────────────────────────────┐
│ [Platform Icon] [Source Badge]      │
│ Mention preview text (100 chars)... │
│ [😊 Positive] [Intent: Praise]      │
│ [Free/Paid indicator]               │
│ 2 hours ago                         │
│ [View Details →]                    │
└─────────────────────────────────────┘
```

**Bottom Section:**

- Pagination or "Load More" button
- Results count: "Showing 1-20 of 156 mentions"

#### 6. **MENTION DETAILS**

**Purpose:** Deep dive into single mention
**URL:** `/mentions/{id}`

**Layout:**

```
Breadcrumb: Dashboard > Mentions > Details

┌─────────────────────────────────────┐
│ ORIGINAL MENTION                    │
│ • Platform: Facebook                │
│ • Author: @username                 │
│ • Posted: Oct 19, 2025 2:30 PM     │
│ • Full text content                 │
│ • [View Original →]                 │
├─────────────────────────────────────┤
│ AI ANALYSIS                         │
│ • Sentiment Bar:                    │
│   [████████░░] Positive 82%        │
│ • Intent: Complaint                 │
│ • Aspects: #Service #Delivery      │
│ • Confidence: High (94%)            │
├─────────────────────────────────────┤
│ AI SUGGESTED REPLY                  │
│ • Generated response text           │
│ • [Edit] [Approve & Send] [Discard] │
├─────────────────────────────────────┤
│ SIMILAR MENTIONS (sidebar)          │
│ • 3 related mention cards           │
└─────────────────────────────────────┘
```

#### 7. **ALERTS PAGE**

**Purpose:** Critical mentions requiring attention
**URL:** `/alerts`

**Header Section:**

- "High-Priority Mentions" title
- Filter: Type dropdown (All, Negative, Complaint, Refund)
- Time filter (Last 24h, Last 7 days, All)

**Alert Cards Grid:**

```
Each Alert Card:
┌─────────────────────────────────────┐
│ ⚠️ CRITICAL ALERT                   │
│ Platform: Google Reviews            │
│ "Terrible service, want refund..."  │
│ Severity: ████░ (4/5)              │
│ Created: 30 mins ago                │
│ [Open Details] [Mark Resolved]      │
└─────────────────────────────────────┘
```

**Notification Log Section:**

- Table showing alert delivery history
- Columns: Time, Channel (Email/SMS/WhatsApp), Status

#### 8. **REPORTS & INSIGHTS**

**Purpose:** Analytics and export
**URL:** `/reports`

**Controls Section:**

- Period selector (Last 7 days, 30 days, 90 days, Custom)
- Platform filter (All or specific)
- Export buttons: [PDF] [CSV] [Excel]

**Charts Grid:**

```
Row 1:
├─ Sentiment Trend (Line Chart)
└─ Platform Distribution (Donut Chart)

Row 2:
├─ Top Complaint Categories (Bar Chart)
└─ Response Rate (Progress Chart)

Row 3:
└─ Auto-generated Summary Card
   "Your sentiment improved 15% this month"
```

#### 9. **INTEGRATIONS**

**Purpose:** Connect platform accounts
**URL:** `/integrations`

**Platform Connection Cards:**

```
Each Integration Card:
┌─────────────────────────────────────┐
│ [Logo] Platform Name                │
│ Status: ● Connected / ○ Disconnected│
│ Method: Official API / Apify        │
│ Cost: Free / Paid (Professional+)   │
│ Last Sync: 2 hours ago              │
│ [Connect] or [Settings|Disconnect]  │
└─────────────────────────────────────┘
```

List of 9 cards:

1. Google Business (API - Free)
2. YouTube (API - Free)
3. Reddit (API - Free)
4. Facebook Page (Graph API - Free)
5. Facebook Public (Apify - Paid)
6. Instagram (Graph API - Free)
7. Instagram Public (Apify - Paid)
8. LinkedIn (Apify - Paid)
9. TikTok (Apify - Paid)

**Bottom Section:**

- Info box: "Data refresh rates and limitations"
- Toggle switches for platform-specific alerts

#### 10. **SETTINGS**

**Purpose:** Account & preferences
**URL:** `/settings`

**Tabs:**

- Profile
- Password
- Notifications
- Billing
- Danger Zone

**Profile Tab:**

- Business Name input
- Email input
- Phone input
- Language selector
- Timezone selector
- [Save Changes] button

**Password Tab:**

- Current Password input
- New Password input
- Confirm Password input
- [Update Password] button

**Notifications Tab:**

- Email notifications toggle
- SMS notifications toggle
- WhatsApp notifications toggle
- Alert frequency selector
- Critical alerts override checkbox

**Billing Tab:**

- Current Plan display
- Next billing date
- Payment method
- [Upgrade Plan] button
- Invoice history table

**Danger Zone:**

- [Export All Data] button
- [Delete Account] button (red)

---

### 👨‍💼 ADMIN PANEL (5 Screens)

#### 11. **ADMIN OVERVIEW**

**Purpose:** System-wide dashboard
**URL:** `/admin`

**KPI Grid:**

- Total Active Businesses
- Total Mentions Processed Today
- Average Sentiment (All Clients)
- System Health Status
- Active Apify Jobs
- API Usage This Month

**Charts:**

- Client Growth (Line)
- Platform Usage Distribution (Bar)
- Revenue Trends (Area)

#### 12. **MANAGE CLIENTS**

**Purpose:** Client administration
**URL:** `/admin/clients`

**Client Table:**
| Business Name | Plan | Last Active | Mentions | Usage | Actions |
|--------------|------|-------------|----------|--------|---------|
| Cafe Aroma | Pro | 2h ago | 1,234 | 85% | [View][Edit][Suspend] |

**Filters:**

- Plan type
- Status (Active, Suspended, Trial)
- Search by name

**Bulk Actions:**

- Export selected
- Send announcement
- Bulk plan change

#### 13. **MONITOR JOBS**

**Purpose:** Apify & API job tracking
**URL:** `/admin/jobs`

**Jobs Table:**
| Job ID | Type | Platform | Client | Status | Started | Duration | Actions |
|--------|------|----------|--------|--------|---------|----------|---------|
| #1234 | Apify | LinkedIn | Cafe X | Running | 14:30 | 2m 15s | [View][Stop] |

**Status Filters:**

- Running
- Completed
- Failed
- Queued

**Controls:**

- [Trigger Manual Run] button
- Auto-refresh toggle
- Retry failed jobs

#### 14. **BILLING & PLANS**

**Purpose:** Subscription management
**URL:** `/admin/billing`

**Sections:**

1. **Plan Overview Table:**

   - Plan features comparison
   - Pricing editor
   - Feature toggles

2. **Client Subscriptions:**

   - Active subscriptions list
   - Expiring soon warnings
   - Grace period clients
   - Manual renewal actions

3. **Revenue Analytics:**
   - MRR chart
   - Churn rate
   - Plan distribution
   - Payment gateway stats

#### 15. **SYSTEM LOGS**

**Purpose:** Activity monitoring
**URL:** `/admin/logs`

**Log Table:**
| Timestamp | User | Action | Endpoint | Status | Response Time |
|-----------|------|--------|----------|--------|---------------|
| 14:32:15 | admin@... | GET | /api/mentions | 200 | 145ms |

**Filters:**

- Log level (Info, Warning, Error)
- User type
- Date range
- Endpoint

---

## 🧩 COMPONENT LIBRARY

### Navigation Components

- **TopBar** - Logo, user menu, notifications
- **Sidebar** - Collapsible navigation menu
- **Breadcrumb** - Navigation path indicator
- **TabBar** - Section navigation

### Data Display Components

- **KPICard** - Metric with icon and trend
- **MentionCard** - Compact mention preview
- **AlertCard** - Priority notification card
- **PlatformBadge** - Platform icon with status
- **SentimentBadge** - Colored sentiment indicator
- **IntentTag** - Intent classification tag

### Input Components

- **SearchBar** - Global search input
- **FilterDropdown** - Multi-select filter
- **DateRangePicker** - Date selection
- **ToggleSwitch** - On/off settings
- **PlanSelector** - Radio button group

### Chart Components

- **LineChart** - Trend visualization
- **PieChart** - Distribution display
- **BarChart** - Comparison view
- **ProgressBar** - Completion indicator
- **SentimentBar** - Positive/negative ratio

### Action Components

- **PrimaryButton** - Main CTAs
- **SecondaryButton** - Alternative actions
- **IconButton** - Compact actions
- **BulkActionBar** - Multiple selection actions
- **ExportButton** - Download options

### Feedback Components

- **Toast** - Temporary notifications
- **Modal** - Confirmation dialogs
- **EmptyState** - No data illustrations
- **ErrorBoundary** - Error messages
- **LoadingSkeleton** - Content placeholders
- **ProgressSpinner** - Loading indicators

### Layout Components

- **PageHeader** - Title and actions
- **Card** - Content container
- **Table** - Data grid
- **Grid** - Responsive layout
- **Section** - Content grouping

---

## 📱 RESPONSIVE BREAKPOINTS

### Desktop (1440px+)

- Full sidebar visible
- Multi-column layouts
- All features enabled

### Tablet (768px - 1439px)

- Collapsible sidebar
- 2-column max layouts
- Touch-optimized buttons

### Mobile (375px - 767px)

- Bottom navigation
- Single column layout
- Stacked cards
- Simplified charts
- Drawer-based filters

---

## 🎨 DESIGN STATES (Per Screen)

For EVERY screen, design these 5 states:

1. **Default State** - Normal with data
2. **Loading State** - Skeleton loaders
3. **Empty State** - No data message + illustration
4. **Error State** - Error message + retry action
5. **Mobile State** - Responsive layout

**Example for Mentions Feed:**

- Default: List of mention cards
- Loading: 5 skeleton cards
- Empty: "No mentions found" + illustration
- Error: "Failed to load" + [Retry] button
- Mobile: Single column + drawer filters

---

## 🔄 USER FLOWS TO MAP

### Flow 1: New User Onboarding

```
Landing → Sign Up → Email Verification →
Initial Setup → Connect First Platform → Dashboard
```

### Flow 2: Responding to Alert

```
Alert Notification → Alerts Page →
Mention Details → Review AI Reply →
Edit → Approve & Send → Mark Resolved
```

### Flow 3: Platform Integration

```
Integrations Page → Select Platform →
OAuth Flow / Apify Setup → Test Connection →
Configure Settings → First Data Sync
```

### Flow 4: Generating Report

```
Reports Page → Select Period →
Apply Filters → View Charts →
Export PDF → Download
```

### Flow 5: Admin Client Management

```
Admin Panel → Manage Clients →
Search Client → View Details →
Change Plan → Confirm → Send Notification
```

---

## 🎯 DESIGN PRIORITIES

### Phase 1 (MVP - Week 1-2)

1. Dashboard
2. Mentions Feed
3. Login/Signup
4. Mention Details
5. Alerts

### Phase 2 (Core - Week 3-4)

6. Integrations
7. Reports
8. Settings
9. Landing Page

### Phase 3 (Admin - Week 5)

10. Admin Overview
11. Manage Clients
12. Monitor Jobs
13. Billing
14. System Logs

---

## ✅ DESIGN DELIVERABLES CHECKLIST

### Per Page (55 total screens):

- [ ] Desktop wireframe
- [ ] Tablet wireframe
- [ ] Mobile wireframe
- [ ] Loading state
- [ ] Empty state
- [ ] Error state

### Component Library:

- [ ] All 40+ components designed
- [ ] Component documentation
- [ ] Interaction states (hover, active, disabled)
- [ ] Dark mode variants (optional)

### Design System:

- [ ] Color palette
- [ ] Typography scale
- [ ] Spacing system (8px grid)
- [ ] Icon library
- [ ] Shadow/elevation system

### Handoff Materials:

- [ ] Figma file organized by pages
- [ ] Component library file
- [ ] Prototype with clickable flows
- [ ] Design tokens for developers
- [ ] Responsive behavior notes

---

## 📏 SIZING GUIDELINES

### Typography

- H1: 32px (Page titles)
- H2: 24px (Section headers)
- H3: 20px (Card titles)
- Body: 16px (Regular text)
- Small: 14px (Metadata)
- Tiny: 12px (Badges)

### Spacing

- Base unit: 8px
- Card padding: 24px
- Section margin: 32px
- Button padding: 12px 24px
- Input height: 40px

### Colors - Purple Theme System

**Primary Purple Palette:**

- Deep Purple: #720e9e (Headers, important CTAs)
- Royal Purple: #8b5cf6 (Primary brand color)
- Medium Purple: #a855f7 (Interactive elements)
- Light Purple: #c084fc (Hover states, accents)
- Pale Purple: #ddd6fe (Backgrounds, subtle tints)

**Semantic Colors:**

- Success: #22c55e / #16a34a (Positive sentiment)
- Error: #ef4444 / #dc2626 (Negative sentiment)
- Warning: #fb923c / #ea580c (Neutral/Warning)
- Info: #60a5fa / #2563eb (Information)

**Light Mode:**

- BG Primary: #ffffff
- BG Secondary: #faf5ff (Purple tint)
- BG Tertiary: #f3e8ff (Stronger purple tint)
- Text Primary: #111827
- Border Purple: #d8b4fe

**Dark Mode:**

- BG Primary: #0f0f1e (Dark purple-tinted)
- BG Secondary: #1a1a2e (Dark purple-gray)
- BG Tertiary: #252542
- Text Primary: #f3f4f6
- Border Purple: #6b21a8

**Gradients:**

- Primary: linear-gradient(135deg, #8b5cf6 0%, #a855f7 100%)
- Hero: linear-gradient(180deg, #faf5ff 0%, #ffffff 100%)
- Dark Hero: linear-gradient(180deg, #0f0f1e 0%, #1a1a2e 100%)

---

## 🚀 IMPLEMENTATION NOTES

1. **Start with Dashboard** - Sets the design language
2. **Design mobile-first** - Easier to scale up
3. **Use real data** - Avoid lorem ipsum
4. **Include micro-interactions** - Loading, hover, transitions
5. **Test with users** - Validate navigation flows
6. **Document edge cases** - What happens when...
7. **Maintain consistency** - Use component library
8. **Consider accessibility** - Color contrast, font sizes

---

## 📊 SUCCESS METRICS

Your UI design is complete when:
✅ All 55 screens are designed
✅ Component library is reusable
✅ Developers can build without clarification
✅ All error states are handled
✅ Mobile experience is optimized
✅ Design system is documented

---

**END OF UI DESIGN ROADMAP**

This roadmap provides your UI team with:

- Complete page inventory
- Detailed component specifications
- Clear navigation structure
- Design state requirements
- Priority order for implementation

Your designers can now start creating wireframes in Figma with full confidence about what needs to be built!
