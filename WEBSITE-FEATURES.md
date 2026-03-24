# Corell - Website Features & Experience

## Project Overview
- **Project Name**: Corell Dynamic Risk Hub
- **Type**: Corporate landing page / Single-page website
- **Industry**: Risk management & security services
- **Design Theme**: Dark cyberpunk with lime green accents

---

## Visual Design Features

### Color Palette
| Role | Color | Hex |
|------|-------|-----|
| Primary Accent | Lime Green | `#ccff00` |
| Primary Dark | Lime Dark | `#b3e600` |
| On Primary | Near Black | `#0a0a0a` |
| Background | Deep Black | `#0a0a0f` |
| Surface | Dark Gray | `#12121a` |
| Surface Light | Lighter Gray | `#1a1a24` |
| On Background | Off White | `#f0f0f5` |
| On Surface | Light Gray | `#d0d0da` |
| Accent Blue | Blue | `#3b82f6` |
| Accent Cyan | Cyan | `#06b6d4` |
| Danger | Red | `#ef4444` |

### Typography
- **Headlines**: Orbitron (futuristic tech font)
- **Body**: Space Grotesk (modern geometric sans)
- **Monospace**: JetBrains Mono (code/technical feel)

### Layout & Spacing
- Max content width: 1600px
- Responsive padding: 1.5rem (mobile) → 3rem (desktop)
- 12-column grid system
- Consistent gap spacing: 4-12 units

---

## Core UI Components

### 1. Navigation Bar
- Fixed position with backdrop blur
- Glass morphism effect (`bg-[#0a0a0fcc] backdrop-blur-xl`)
- Border-bottom: subtle white/5
- Logo with hover scale/rotate animation
- Active state with pulsing dot indicator
- Mobile hamburger menu with animated lines

### 2. Mobile Menu
- Full-screen overlay (`transform: translateX(100%)`)
- Slide-in animation (0.5s ease-out)
- Backdrop blur effect
- Staggered navigation links
- Status card at bottom
- CTA button

### 3. Glass Cards
- Gradient background (rgba 18,18,26 → 26,26,36)
- Backdrop filter blur (20px)
- Border: 1px solid rgba(255,255,255,0.05)
- Box shadow: 0 25px 50px -12px rgba(0,0,0,0.5)

### 4. Modular Border Cards
- Gradient background
- Border with white/10 opacity
- Corner accent decorations (40px×40px)
- Hover effect: lime green border glow
- Top border line animation on hover

### 5. Buttons
#### Primary Button
- Gradient: `#ccff00` → `#b3e600`
- Orbitron font, bold, uppercase
- Hover: scale(1.05) + box-shadow glow
- Rounded corners (lg)

#### Secondary Button
- Transparent with border
- Hover: border turns lime green + bg rgba(204,255,0,0.1)

### 6. Stat Numbers
- Gradient text effect (lime green)
- Large font sizes (5xl-7xl)
- Orbitron black weight

### 7. Corner Accents
- 40×40px decorative elements
- Lime green at 30% opacity
- Four positions: top-left, top-right, bottom-left, bottom-right
- Borders create geometric corner effect

### 8. Scan Line Animation
- Horizontal gradient line (lime green 60% opacity)
- Repeating vertical scan animation (3s)
- Used in backgrounds for depth

---

## Background Effects

### Cyber Background
- Linear gradient: #0a0a0f → #12121a
- Grid pattern overlay (60×60px, rgba lime 2%)
- Fixed position, pointer-events none

### Geometric Pattern
- SVG hexagon/diamond pattern
- 60×60px repeating
- Very low opacity (5%)
- Used throughout sections

### Ambient Blobs
- Large blur gradients (3xl)
- Lime/blue at 10% opacity
- Float animation
- Positions: top-right, bottom-left, bottom-right

---

## Animation System

### Keyframe Animations
| Name | Duration | Easing | Description |
|------|----------|--------|-------------|
| fadeIn | 0.8s | ease-out | Opacity 0→1 |
| slideUp | 0.8s | ease-out | Opacity 0→1 + translateY 40px→0 |
| float | 6s | ease-in-out | translateY + rotate oscillation |
| scan | 3s | linear | Vertical gradient sweep |
| pulse-slow | 4s | ease-in-out | Standard pulse |

### Stagger Delays
- `.stagger-1`: 0.1s
- `.stagger-2`: 0.2s
- `.stagger-3`: 0.3s
- `.stagger-4`: 0.4s
- `.stagger-5`: 0.5s
- `.stagger-6`: 0.6s

---

## Section Breakdown

### 1. Hero Section (#home)
- Full viewport height (min-h-screen)
- Two-column layout: content (8 cols) + live feed card (4 cols)
- "Active Surveillance Mode" badge with pulsing indicator
- Version tag
- Large headline with gradient highlight
- Description paragraph
- Two CTA buttons (primary + secondary)

### 2. Live Feed Card
- Glass card styling
- Corner accents
- Live indicator with red pulse
- Three feed items with icons
- Processing load progress bar (67%)

### 3. Features Section (#features)
- Integrated Response Vectors
- 4-column grid layout with varying spans (8, 4, 5, 7)
- Monitoring card with stats (latency, endpoints, alert level)
- Intelligence/Threat Matrix card with scan button
- Adaptive Protocols card with metrics
- Logistics card with globe icon

### 4. Stats Section
- Three large stat cards: 99.999% uptime, 84k+ nodes, 12M+ threats
- Blockquote with gradient accent
- Secure link visualization card

### 5. About Section (#about)
- Two-column layout
- Visual card with "Command Node" detail
- "Proactive Risk Architects" headline
- Three feature cards with icons

### 6. Services Section (#services)
- "Onboarding Sequence" title
- 7-step horizontal grid (sm → md → lg responsive)
- Each step: code (S_01-S_06, OPTIMIZED), title, description
- Last card has gradient + corner accent

### 7. Intelligence Section
- Two columns: blog posts + FAQ
- Blog cards with date, title, excerpt
- FAQ accordion-style with add icon
- Hover effects on cards

### 8. Contact Section (#contact)
- Multi-field form (Name, Email, Organization, Message)
- Glass card styling
- Form fields with dark background
- Submit button with arrow icon

### 9. Footer
- Three-column layout (logo + nav + contact)
- Social links with icon circles
- Copyright text
- Gradient top border

---

## Responsive Breakpoints
- **Mobile**: < 640px (1 column, mobile menu)
- **Tablet**: 640px - 1023px (2 columns)
- **Desktop**: 1024px - 1279px (full nav, 12-col grid)
- **XL**: 1280px+ (larger padding, full effects)

---

## User Experience Features

### Navigation
- Smooth scroll to sections via anchor links
- Active state highlighting on scroll (via URL hash)
- Mobile menu accessible via hamburger
- Status indicator always visible

### Interactivity
- All cards have hover states (border color, glow)
- Buttons scale and glow on hover
- Navigation links have underline animation
- Mobile menu slides smoothly

### Accessibility Considerations
- Semantic HTML (nav, main, section, article, footer)
- Alt text on icons (via aria-label where needed)
- Sufficient color contrast (lime on dark)
- Focus states on interactive elements
- Reduced motion support via CSS

### Performance
- Tailwind CDN for rapid styling
- No external JS frameworks
- SVG icons (inline)
- CSS animations (GPU accelerated)
- Optimized fonts (Google Fonts)

---

## Technical Implementation

### External Dependencies
- Tailwind CSS (CDN)
- Google Fonts (Orbitron, Space Grotesk, JetBrains Mono)
- Material Symbols Outlined (Google Fonts)

### CSS Custom Properties
- All colors defined in Tailwind config
- Custom animations in keyframes
- Glass morphism effects via backdrop-filter

### File Structure
- Single `index.html` file
- All CSS inline in `<style>` tag
- Tailwind config in `<script>` tag
- No build process required

---

## Design System Summary

### Aesthetic
- Futuristic / Command center / Cyberpunk
- Professional but cutting-edge
- Trustworthy for risk management

### Key Visual Motifs
- Lime green accent (#ccff00)
- Geometric corners and patterns
- Scan line animations
- Glass/glassmorphism effects
- Grid background overlay

### Tone
- Technical, precise
- Authoritative
- Modern, forward-thinking
- Security-focused

---

*Generated for Corell Dynamic Risk Hub - Website Features & Experience Documentation*
