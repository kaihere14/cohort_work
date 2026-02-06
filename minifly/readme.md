
# Minifly - Mintlify Clone

A pixel-perfect recreation of the Mintlify landing page, built with vanilla HTML and CSS. This project demonstrates modern web design principles, responsive layouts, and clean code architecture.

![Minifly Preview](https://img.shields.io/badge/Status-Complete-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)

## 🎯 Project Overview

This is a static website clone of Mintlify's landing page, featuring:

- Modern, clean design with smooth animations
- Fully responsive layout
- Semantic HTML structure
- Custom CSS styling without frameworks
- Interactive elements and hover effects

## 📋 Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Step-by-Step Build Process](#step-by-step-build-process)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Deployment](#deployment)
- [Lessons Learned](#lessons-learned)

## ✨ Features

### Navigation

- Fixed navigation bar that stays visible on scroll
- Transparent background with backdrop blur effect
- Responsive navigation links
- Call-to-action buttons (Contact Sales, Start for Free)

### Hero Section

- Eye-catching gradient background
- "NEW" badge with announcement
- Large, bold typography
- Email input with integrated CTA button
- Product screenshot showcase

### Companies Section

- Trusted companies logo showcase

### Features Section

- Multi-column feature cards
- Icon integration
- Large feature card with extended content
- Responsive grid layout

### Enterprise Section

- Enterprise-focused content
- Icon-based feature cards
- Customer story highlight (Anthropic case study)
- Statistics display
- Company logos showcase

### Customers Section

- Customer story grid (3 columns)
- Image cards with descriptions
- Navigation controls
- Call-to-action section

### CTA Split Section

- Two-column layout with divider
- Icon-based CTAs
- Pricing and Quickstart links

### Footer

- Multi-column navigation (5 columns)
  - Explore
  - Resources
  - Documentation
  - Company
  - Legal
- Social media links (LinkedIn, X, GitHub)
- Security badge (AICPA SOC 2)
- System status indicator
- Theme toggle buttons
- Copyright information

## 📁 Project Structure

```
Minifly/
├── index.html          # Main HTML file
├── style.css           # All styling
├── README.md           # Project documentation
└── Assets/
    ├── images/         # All image assets
    │   ├── Mintlify_idjQU-FEBd_1.svg
    │   ├── bg-light.svg
    │   ├── hero-image-light.svg
    │   ├── trusted.png
    │   ├── features-1.png
    │   ├── features-2.png
    │   ├── features-3.png
    │   ├── anthropic.svg
    │   ├── enter-companies.png
    │   ├── perplexity.webp
    │   ├── x.webp
    │   └── kalshi.webp
    └── fonts/
        └── Inter-VariableFont_slnt,wght.ttf
```

## 🛠️ Step-by-Step Build Process

### Phase 1: Project Setup & Foundation

#### Step 1: Initialize Project Structure

```bash
mkdir Minifly
cd Minifly
touch index.html style.css README.md
mkdir -p Assets/images Assets/fonts
```

#### Step 2: Set Up HTML Boilerplate

- Created basic HTML5 structure
- Added meta tags for viewport and charset
- Linked external CSS file
- Added favicon
- Set up semantic HTML structure with `<nav>`, `<main>`, `<section>`, `<footer>`

#### Step 3: Import Custom Font

- Downloaded Inter font (Variable font)
- Added `@font-face` rule in CSS
- Set Inter as the default font family

#### Step 4: CSS Reset & Variables

```css
/* Reset default styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Define CSS variables */
:root {
  --primary-color: #08090b;
  --secondary-color: #ffffff;
  --mountain-meadow: #18e299;
  --riptide: #3f8a62;
  --bg-light: #ffffff;
  --border-color: rgba(0, 0, 0, 0.08);
  --text-main: #08090b;
  --text-muted: rgba(62, 61, 61, 0.9);
}
```

### Phase 2: Navigation Bar

#### Step 5: Build Navigation HTML

- Created `<nav>` element with three sections:
  - Logo container
  - Navigation links (Resources, Documentation, Customers, Blog, Pricing)
  - Login buttons (Contact Sales, Start for Free)

#### Step 6: Style Navigation

- Set `position: sticky` (later changed to `fixed`)
- Added backdrop blur effect
- Styled navigation links with proper spacing
- Created button styles with hover effects
- Fixed navigation bar visibility issue by:
  - Changing from `sticky` to `fixed` positioning
  - Adding semi-transparent background color
  - Ensuring proper z-index layering

### Phase 3: Hero Section

#### Step 7: Create Hero Background

- Added `.back-image` container with SVG background
- Set background properties (cover, top positioning)
- Ensured minimum height of 100vh

#### Step 8: Build "NEW" Badge

- Created update notification badge
- Styled with rounded corners and icon
- Added green "NEW" label with proper spacing

#### Step 9: Hero Content

- Added large heading with line break
- Created subtitle with proper opacity
- Built email input wrapper with:
  - Transparent input field
  - Integrated "Start now" button
  - Glassmorphism effect (backdrop blur)
  - Rounded pill shape

#### Step 10: Add Hero Image

- Positioned product screenshot
- Added border radius for modern look
- Ensured responsive sizing

### Phase 4: Companies Section

#### Step 11: Companies Showcase

- Added trusted companies image
- Set full-width display
- Ensured proper spacing from hero section

### Phase 5: Features Section

#### Step 12: Features Header

- Created centered heading and description
- Set proper typography and spacing
- Limited description width for readability (38%)

#### Step 13: Feature Cards

- Built two-column grid layout
- Created card component with:
  - Label (uppercase, green color)
  - Heading
  - Description
  - Feature image
- Added border and border-radius
- Set minimum height for consistency

#### Step 14: Big Feature Card

- Created larger, centered card
- Adjusted width to 68%
- Centered text alignment
- Wider description (52% max-width)

### Phase 6: Enterprise Section

#### Step 15: Enterprise Title Section

- Created two-part title layout:
  - Main title with green label
  - Subtitle with CTA button
- Styled with flexbox for proper alignment

#### Step 16: Enterprise Cards

- Built two-column card layout
- Added SVG icons with green color
- Created card content structure
- Set proper spacing and typography

#### Step 17: Anthropic Case Study

- Added background image
- Created two-section layout (upper/lower)
- Upper section:
  - Label, heading, and CTA link
  - Rotated arrow icon
- Lower section:
  - Statistics display (2M+ users, 3+ products)
  - Proper spacing and color contrast

#### Step 18: Enterprise Companies

- Added company logos showcase
- Set proper padding and spacing

### Phase 7: Customers Section

#### Step 19: Customers Header

- Added label, title, and subtitle
- Centered alignment
- Limited subtitle width (40%)

#### Step 20: Customer Stories Grid

- Created 3-column grid layout
- Built customer item cards with:
  - Image (394x290px, rounded corners)
  - Description text
  - "Read story" link
- Added proper gap spacing

#### Step 21: Navigation Buttons

- Created circular navigation buttons
- Added SVG icons (left/right arrows)
- Styled with different colors (gray/black)
- Rotated right arrow 180 degrees

#### Step 22: Start Buttons Section

- Added large heading and description
- Created two CTA buttons:
  - "Get started for free" (filled)
  - "Get a demo" (outlined)
- Styled with rounded pill shape

### Phase 8: CTA Split Section

#### Step 23: Two-Column CTA Layout

- Created grid layout with divider
- Built two CTA boxes:
  - Pricing CTA (left)
  - Quickstart CTA (right)
- Added SVG icons with background
- Styled links with hover effects

### Phase 9: Footer

#### Step 24: Footer Structure

- Created footer container with max-width
- Added light gray background (#f8f8f8)
- Set proper padding and borders

#### Step 25: Footer Top Section

- Added Mintlify logo (filtered to black)
- Created social media icons:
  - LinkedIn
  - X (Twitter)
  - GitHub
- Added hover effects

#### Step 26: Footer Navigation

- Created 5-column grid layout:
  - Explore
  - Resources
  - Documentation
  - Company
  - Legal
- Styled headings (uppercase, gray, small)
- Added link hover effects (green color)

#### Step 27: Security Badge

- Added "Backed By Enterprise-Grade Security" text
- Created AICPA SOC 2 badge
- Styled with border and padding

#### Step 28: Footer Bottom Bar

- Created three-section layout:
  - System status (green indicator dot)
  - Copyright (centered)
  - Theme toggles (3 buttons)
- Added theme button icons:
  - System (monitor icon)
  - Light (sun icon)
  - Dark (moon icon)
- Styled with hover effects

### Phase 10: Refinements & Polish

#### Step 29: Responsive Adjustments

- Adjusted padding and margins
- Fixed overflow issues (`overflow-x: hidden`)
- Ensured proper spacing throughout

#### Step 30: Final Touches

- Updated favicon to official Mintlify icon
- Removed unnecessary comments
- Cleaned up code formatting
- Tested all hover effects
- Verified color consistency

## 💻 Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with:
  - Flexbox
  - CSS Grid
  - Custom properties (variables)
  - Backdrop filters
  - Transitions and hover effects
- **Google Fonts**: Inter (Variable font)
- **SVG**: Icons and graphics

## 🚀 Installation

1. **Clone the repository**

```bash
git clone https://github.com/testingaccount2008/minifly_work.git
cd minifly_work
```

2. **Open in browser**

```bash
# Simply open index.html in your browser
open index.html
# or
# Use a local server (recommended)
python -m http.server 8000
# Then visit http://localhost:8000
```

## 🌐 Deployment

This project can be deployed to any static hosting service:

### GitHub Pages

1. Push code to GitHub repository
2. Go to Settings > Pages
3. Select main branch
4. Your site will be live at `https://yourusername.github.io/minifly_work`

### Netlify

1. Drag and drop the project folder to Netlify
2. Or connect your GitHub repository
3. Deploy automatically

### Vercel

```bash
npm i -g vercel
vercel
```

## 📚 Lessons Learned

### Design Principles

1. **Consistency is key**: Using CSS variables ensures consistent colors throughout
2. **Spacing matters**: Proper padding and margins create visual hierarchy
3. **Typography**: Font size, weight, and line-height significantly impact readability

### Technical Insights

1. **Fixed vs Sticky positioning**: Fixed positioning works better for always-visible navbars
2. **Backdrop filters**: Create modern glassmorphism effects
3. **CSS Grid**: Perfect for multi-column layouts (footer, features)
4. **Flexbox**: Ideal for navigation bars and single-direction layouts
5. **SVG icons**: Scalable and customizable with CSS

### Challenges Overcome

1. **Navigation bar hiding**: Solved by switching from sticky to fixed positioning
2. **Color consistency**: Implemented CSS variables for easy theme management
3. **Responsive images**: Used proper sizing and object-fit properties
4. **Hover effects**: Added smooth transitions for better UX

## 🎨 Design Decisions

### Color Palette

- **Primary**: #08090B (Almost black)
- **Secondary**: #FFFFFF (White)
- **Accent**: #18E299 (Mint green)
- **Muted**: rgba(62, 61, 61, 0.9) (Gray)

### Typography

- **Font Family**: Inter (Variable)
- **Headings**: 600 weight, larger sizes
- **Body**: 400 weight, 16px base
- **Labels**: 12px, uppercase, letter-spacing

### Layout

- **Max Width**: 1200px for content containers
- **Padding**: 2rem horizontal, 4rem vertical for sections
- **Gap**: 2-3rem for grid layouts
- **Border Radius**: 20-24px for cards, 50-100px for buttons

## 🔧 Future Enhancements

- [ ] Add JavaScript for interactive elements
- [ ] Implement theme switcher functionality
- [ ] Add smooth scroll animations
- [ ] Create mobile hamburger menu
- [ ] Add form validation
- [ ] Implement carousel for customer stories
- [ ] Add loading animations
- [ ] Create dark mode variant

## 👨‍💻 Author

Built with ❤️ by [testingaccount2008](https://github.com/testingaccount2008)

## 📄 License

This project is for educational purposes only. All design credits go to [Mintlify](https://mintlify.com).

## 🙏 Acknowledgments

- Design inspiration: [Mintlify](https://mintlify.com)
- Font: [Inter by Rasmus Andersson](https://rsms.me/inter/)
- Icons: Custom SVG implementations

---

**Note**: This is a clone project created for learning purposes. It is not affiliated with or endorsed by Mintlify.
