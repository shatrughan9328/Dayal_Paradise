# 🏨 Hotel Dayal Paradise – 4-Star Luxury Hotel Website

> **A plush address of Comfort, Serenity, Luxury & Greenery in Gomti Nagar, Lucknow.**  
> Official web portal featuring signature room reservations, royal Awadhi dining showcases, grand banquet planning, and an interactive guest experience engine.

---

## 📌 Table of Contents
1. [Executive Summary](#-executive-summary)
2. [Project Highlights & Features](#-project-highlights--features)
3. [Technology Stack](#-technology-stack)
4. [File & Directory Architecture](#-file--directory-architecture)
5. [Page-by-Page Breakdown](#-page-by-page-breakdown)
6. [Design System & Style Guide](#-design-system--style-guide)
7. [Interactive JavaScript Features](#-interactive-javascript-features)
8. [Local Development & Setup](#-local-development--setup)
9. [Deployment Guide](#-deployment-guide)
10. [Hotel Contact & Landmark References](#-hotel-contact--landmark-references)
11. [Developer Interview Questions & Answers (`INTERVIEW_QA.md`)](./INTERVIEW_QA.md)
12. [Project Pitch Scripts & Advanced Technical Guide (`PROJECT_PITCH_AND_ADVANCED_QUESTIONS.md`)](./PROJECT_PITCH_AND_ADVANCED_QUESTIONS.md)

---

## 🌟 Executive Summary

**Hotel Dayal Paradise** is a premier 4-star boutique hotel situated in the tranquil greens of **Vipul Khand, Gomti Nagar, Lucknow**. Catering to discerning business executives, royal destination weddings, leisure travelers, and families, the hotel combines age-old Awadhi Tehzeeb (hospitality) with modern contemporary luxury.

This web project represents a complete, responsive, high-performance web presence crafted using modern front-end technologies. It delivers an intuitive digital concierge experience with real-time room inquiry routing, WhatsApp reservation engines, table bookings, banquet inquiries, and interactive visual galleries.

---

## 🚀 Project Highlights & Features

- **Royal Champagne & Obsidian Aesthetics**: Tailored color palette blending warm gold gradients (`#d4af37`, `#c5a059`) with midnight obsidian (`#080c16`, `#0f172a`) and glassmorphic cards.
- **Floating Real-Time Quick Booking Bar**: Instant check-in/check-out date pickers with auto-calculated defaults and pre-filled room selection.
- **Direct WhatsApp API Integration**: All forms (Room Reservations, Dining Table Bookings, and Banquet Inquiries) format and dispatch formatted requests directly to the hotel reception (`+91 8795838030`).
- **Complete Multi-Page Architecture**: 6 interconnected pages with persistent luxury navigation, mobile drawer menu, and active-state indicators.
- **Dynamic Swiper Coverflow & Lightbox**: 3D coverflow carousel for visual tours and a full-screen interactive lightbox modal for high-res photo viewing.
- **Landmark Driving Directions**: Solved location divider issue with visual travel metric cards (CCS Airport, Charbagh Railway Station, Ekana Cricket Stadium, Gomti Riverfront).
- **Zero-Dependency Components**: Custom accordions, modals, and mobile menus written in clean vanilla ES6+ JavaScript—no bloated UI framework dependencies.
- **Fixed Duplications**: Transformed placeholder duplicates into authentic content (distinct room tiers, 4 experience pillars, authentic banquet capacities, and verified guest testimonials).

---

## 🛠️ Technology Stack

| Technology | Purpose | Implementation Details |
| :--- | :--- | :--- |
| **HTML5** | Semantic Structure | SEO meta tags, ARIA accessibility attributes, clean sectioning |
| **Tailwind CSS v4** | Utility Styling | Rapid utility composition loaded via CDN (`@tailwindcss/browser@4`) |
| **Vanilla CSS3** | Custom Design System | `css/style.css` defining CSS custom properties, glassmorphism, animations |
| **Google Fonts** | Luxury Typography | `Cinzel` & `Playfair Display` (Headings), `Plus Jakarta Sans` (Body text) |
| **Font Awesome 6.5.1**| Vector Icons | Navigation, amenities, contact icons, and social badges |
| **Swiper JS v11** | Carousels | Coverflow 3D photo effects and responsive touch-swipe carousels |
| **Vanilla JavaScript (ES6+)** | Logic & Interactions | Booking modal controller, WhatsApp message builder, custom accordion, lightbox |

---

## 📂 File & Directory Architecture

```text
Dayalparadise/
│
├── css/
│   └── style.css            # Central luxury design system, CSS variables & components
│
├── images/                  # High-resolution media assets (55 total files)
│   ├── 1.jpg, 2.jpg         # Hero carousel slides
│   ├── slidder1.jpg - 4.jpg # Deluxe, Club, Executive, Presidential room images
│   ├── card1.png - 4.png    # 4 Signature experience highlight icons
│   ├── b&l1.jpg - 3.jpg     # Jalsa, Jashn, and Lawn banquet photos
│   ├── dining.jpg, dinner.jpg # Aadab restaurant and Jannat rooftop imagery
│   ├── nitinarora.png, etc. # Verified guest testimonial portraits
│   ├── grid1.jpg - 8.jpg    # Swiper coverflow gallery photos
│   ├── logo.png             # Main hotel logo
│   └── footerlogo.png       # Dark-theme footer logo
│
├── index.html               # Main Homepage & digital concierge portal
├── aboutus.html             # Hotel heritage, DAYAL ethos & mission timeline
├── dining.html              # Aadab restaurant, Jannat rooftop & table reservations
├── b&l.html                 # Jalsa, Jashn, and Royal Lawn banquet showcase
├── aminities.html           # 10 Curated 4-star amenities and wellness facilities
├── gallery.html             # Categorized photo gallery with interactive lightbox
├── index2.html              # Standalone Swiper testing sandbox
├── README.md                # Detailed project documentation and developer guide
├── INTERVIEW_QA.md          # 20+ Detailed technical & architectural interview Q&As
└── PROJECT_PITCH_AND_ADVANCED_QUESTIONS.md # Spoken pitches (30s, 60s, 2min) & deep questions
```

---

## 📄 Page-by-Page Breakdown

### 1. `index.html` (Homepage)
The core digital portal designed to captivate visitors with luxury hotel aesthetics:
- **Top Notification Bar**: Click-to-call (`tel:+918795838030`), click-to-email, location pin to Google Maps, social icons, and *"Book Your Stay"* CTA button.
- **Glassmorphic Navbar**: Backdrop-blur sticky navigation bar with active indicators, brand logo, and a zero-dependency responsive mobile hamburger drawer.
- **Hero Carousel**: Multi-slide luxury banner with automatic crossfade, regal titles, value propositions, and direct action buttons (*"Book Online"*, *"Explore Suites"*).
- **Floating Quick Booking Bar**: Sits elevated over the hero banner. Captures check-in, check-out, room category, and guest counts with auto-defaulted dates.
- **Welcome & 4 Experience Pillars**: Introduces Gomti Nagar’s crown jewel with 4 distinct cards:
  1. *Opulent Rooms & Suites*
  2. *Aadab Fine Dining*
  3. *Banquets & Lawns*
  4. *Wellness & Concierge*
- **Rooms & Signature Suites Showcase**: 4 distinct room tiers with real pricing, amenity tags, strike-through rates, and a smooth horizontal scrollbar:
  - *Deluxe Room* (₹4,499/night)
  - *Club Room* (₹5,999/night)
  - *Executive Suite* (₹7,999/night)
  - *Presidential Suite* (₹12,999/night)
- **Milestones Parallax Banner**: Parallax counter displaying *15,000+ Guests*, *500+ Weddings*, *4.3★ Rating*, and *100% Awadhi Warmth*.
- **Driving Directions & Landmark Distances**: Visual cards displaying driving distance and time to Chaudhary Charan Singh Airport (23.3 Km), Charbagh Railway Station (9.8 Km), Ekana Stadium (6.5 Km), and Gomti Riverfront (3.5 Km) with a direct Google Maps trigger.
- **Core Values Interactive Accordion**: Smooth expand/collapse panels explaining *"What DAYAL Stands For"*, *"Our Mission"*, and *"Our Vision"*.
- **Coverflow Gallery Swiper**: 3D coverflow carousel showcasing hotel highlights.
- **Verified Guest Testimonials**: Authentic reviews hooked to real guest portraits (`nitinarora.png`, `neerajtripathi.png`, `kashish.png`).
- **Responsive 4-Grid Experience**: Visual showcase of Accommodation, Conference, Amenities, and Dining with zoom hover effects.
- **Footer Section**: 4-column comprehensive footer with contact details, quick links, and copyright notice.
- **Floating Action Buttons**: Fixed bottom-right corner buttons for instant WhatsApp chat and mobile phone calling.
- **Quick Reservation Modal**: Overlay modal for booking inquiries with instant WhatsApp dispatcher.

---

### 2. `aboutus.html` (About Us)
Highlights the story, heritage, and values of Dayal Paradise:
- **Breadcrumb Hero**: Ambient banner with title and breadcrumb navigation.
- **Hotel Overview**: Detailed narrative of the hotel's founding in Vipul Khand, Gomti Nagar.
- **Highlight Quote Banner**: Elegant serif quote highlighting the rooftop experience.
- **Photo Mosaic & Heritage Timeline**: Asymmetric grid pairing hotel interior photos with the *15+ Years of Royal Hospitality* milestone badge.
- **DAYAL Ethos Accordion**: Complete explanation of the hotel's name acronym.
- **Guest Impressions Slider**: Testimonials from corporate and vacation guests.

---

### 3. `dining.html` (Dining & Rooftop Jannat)
Dedicated to the culinary offerings of the hotel:
- **Aadab Multi-Cuisine Restaurant**: 60-cover lobby-level dining hall serving authentic Awadhi dum pukht, Mughlai, Indian, and continental cuisines. Highlights separate vegetarian and non-vegetarian kitchens.
- **Jannat Rooftop Restaurant & Bar**: Al fresco rooftop lounge overlooking Gomti Nagar, featuring sizzlers, grilled specialties, and handcrafted beverages.
- **Meal Schedule & Operational Hours**: Visual cards detailing *Breakfast Buffet (07:00 AM – 10:30 AM)*, *Executive Lunch (12:30 PM – 03:30 PM)*, and *Royal Dinner (07:30 PM – 11:30 PM)*.
- **Interactive Table Reservation Engine**: Form allowing guests to choose meal timing, venue preference (Aadab vs. Jannat), guest count, and occasion, automatically generating a WhatsApp reservation request.

---

### 4. `b&l.html` (Banquets & Lawns)
Showcases event venues for destination weddings, summits, and social galas:
- **Jalsa Banquet Hall**: Grand ballroom accommodating up to 500 guests (Theater style: 180, U-shape: 70, Floating: 500).
- **Jashn Banquet Hall**: Lawn-facing intimate hall accommodating up to 150 guests (Theater style: 80, U-shape: 35, Floating: 150).
- **The Royal Paradise Lawn**: Sprawling lush green lawn with a permanent stage setup and dedicated food production area, hosting up to 1,000+ guests.
- **Wedding & Event Inquiry Engine**: Interactive form capturing event type, venue choice, date, and guest count with WhatsApp dispatch.

---

### 5. `aminities.html` (Amenities & Facilities)
Curated grid presenting 10 distinct 4-star hotel facilities:
1. *Aadab Restaurant* (Multi-cuisine dining)
2. *Jannat Rooftop* (Open-air restro-bar)
3. *Plush Bedding* (Custom Queen/Twin beds with luxury linens)
4. *Executive Boardroom* (Conferencing & AV tools)
5. *Grand Banquets* (Jalsa & Jashn celebratory halls)
6. *Lush Green Lawn* (1,000+ guest wedding venue)
7. *Fitness Center* (Gym with cardio & strength machines)
8. *Business Center* (Secretarial & workstation support)
9. *High-Speed Wi-Fi* (Complimentary fiber-optic internet)
10. *Valet Parking* (Secure on-site 24/7 parking)

---

### 6. `gallery.html` (Photo Gallery)
An interactive visual showcase:
- **Category Filter Tabs**: Smooth client-side filtering for:
  - *All Photos*
  - *Rooms & Suites*
  - *Dining & Bar*
  - *Banquets & Lawn*
  - *Exterior & Ambiance*
- **Interactive Lightbox Modal**: Clicking any image opens a full-screen high-resolution modal with caption display, backdrop-dimming, and keyboard/click closing.

---

## 🎨 Design System & Style Guide

All design tokens are defined in [`css/style.css`](file:///c:/Users/asus/OneDrive/Desktop/projects/Dayalparadise/css/style.css):

### Color Palette

| Token Name | Hex Code | Visual Preview | Application |
| :--- | :--- | :--- | :--- |
| `--color-dark` | `#080c16` | Dark Midnight | Section backgrounds, contrast containers |
| `--color-primary` | `#0a1128` | Royal Navy | Headers, footers, primary brand surfaces |
| `--color-dark-card`| `#111827` | Deep Obsidian | Luxury card backgrounds |
| `--gold-primary` | `#c5a059` | Warm Champagne | Accent borders, icons, badge highlights |
| `--gold-light` | `#e5c583` | Light Champagne | Subtitles, hover highlights, active states |
| `--gold-dark` | `#9e7b39` | Antique Gold | Gradient ends, border shadows |
| `--bg-cream` | `#faf7f2` | Warm Ivory | Quote blocks, neutral content surfaces |
| `--bg-sand` | `#f1f5f9` | Slate Tint | Tag backgrounds, subtle divider lines |

### Typography Scale

- **Regal Headings**: `'Cinzel', serif` — used for `h1`, `h2`, `h3`, and luxury card headers.
- **Editorial Serif**: `'Playfair Display', serif` — used for quotes, italic accents, and taglines.
- **Body & Controls**: `'Plus Jakarta Sans', sans-serif` — used for paragraphs, buttons, navigation links, and forms.

### Component Classes

- `.btn-gold`: Shimmer button with gold gradient background, dark text, and dynamic hover light beam.
- `.btn-gold-outline`: Sleek transparent button with 1.5px gold border that fills on hover.
- `.luxury-navbar`: Fixed glassmorphism bar (`backdrop-filter: blur(16px)`) with subtle gold bottom border.
- `.luxury-card`: Dark obsidian card with top gold gradient line that glows on hover.
- `.room-card`: Clean off-white card with smooth image zoom and structured price badges.
- `.custom-accordion-item`: Zero-dependency collapsible panel with animated rotating gold arrow.

---

## ⚡ Interactive JavaScript Features

### 1. Date Prefill Logic
```javascript
// Automatically initializes check-in as today and check-out as tomorrow
const today = new Date();
const tomorrow = new Date(today);
tomorrow.setDate(tomorrow.getDate() + 1);

const formatDate = (date) => date.toISOString().split('T')[0];
// Sets min and default values on inputs
```

### 2. WhatsApp Direct Inquiry Generator
```javascript
// Formats booking parameters into a clean URL-encoded WhatsApp message
const message = `*Hotel Dayal Paradise - Room Reservation Inquiry*%0A%0A` +
  `*Guest Name:* ${encodeURIComponent(name)}%0A` +
  `*Phone:* ${encodeURIComponent(phone)}%0A` +
  `*Check-In:* ${checkIn}%0A` +
  `*Check-Out:* ${checkOut}%0A` +
  `*Room Category:* ${encodeURIComponent(roomType)}%0A` +
  `*Guests:* ${encodeURIComponent(guests)}%0A` +
  `*Special Requests:* ${encodeURIComponent(notes)}`;

window.open(`https://wa.me/918795838030?text=${message}`, '_blank');
```

### 3. Lightbox Engine (`gallery.html`)
- Opens clicked photo at native resolution.
- Shows dynamic photo caption.
- Closes via close button (`X`) or clicking the dark backdrop.

### 4. Interactive Accordion Toggle
```javascript
function toggleAccordion(button) {
  const item = button.closest('.custom-accordion-item');
  const isActive = item.classList.contains('active');
  document.querySelectorAll('.custom-accordion-item').forEach(acc => acc.classList.remove('active'));
  if (!isActive) item.classList.add('active');
}
```

---

## 💻 Local Development & Setup

This is a static, lightweight project requiring no server-side compilation or `npm install` build step.

### Method 1: Direct File Opening
Double-click `index.html` in your file explorer or open it via any browser:
```bash
# Windows PowerShell
Start-Process "c:\Users\asus\OneDrive\Desktop\projects\Dayalparadise\index.html"
```

### Method 2: VS Code Live Server
1. Open the folder in **Visual Studio Code**.
2. Install the **Live Server** extension (by Ritwick Dey).
3. Right-click `index.html` and select **"Open with Live Server"** (runs at `http://127.0.0.1:5500`).

### Method 3: Node.js Static Server
If Node.js is installed:
```bash
npx serve . -l 3000
# Open http://localhost:3000 in your browser
```

---

## 🌐 Deployment Guide

This project can be deployed instantly to any modern static hosting provider:

### 1. GitHub Pages
1. Push this repository to GitHub.
2. In your repository, go to **Settings** > **Pages**.
3. Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
4. Click **Save**. The website will be live in 60 seconds at `https://<username>.github.io/<repo-name>/`.

### 2. Vercel
1. Install Vercel CLI: `npm i -g vercel`.
2. Run `vercel` in the project root directory.
3. Accept defaults for static site deployment.

### 3. Netlify
1. Drag and drop the `Dayalparadise/` folder into the [Netlify Drop](https://app.netlify.com/drop) dashboard.
2. Deployment completes automatically with an instant HTTPS URL.

---

## 📞 Hotel Contact & Landmark References

- **Physical Address**: Hotel Dayal Paradise, Vipul Khand - V, Gomti Nagar, Lucknow, Uttar Pradesh 226010, India
- **Front Desk Reservation**: `+91 8795838030`
- **Landline Reception**: `+91 (522) 405 9999`
- **Home Delivery / In-Room Dining**: `+91 9235259906` / `+91 9235259907`
- **Email Contact**: `reservation@dayalparadise.com`
- **Check-in / Check-out**: Check-in from 12:00 PM | Check-out by 11:00 AM

### Strategic Travel Distances
- **Chaudhary Charan Singh International Airport (LKO)**: 23.3 Km (~35 mins via Shaheed Path)
- **Charbagh Railway Station (LKO)**: 9.8 Km (~20 mins via Lohia Path)
- **Bharat Ratna Shri Atal Bihari Vajpayee Ekana Cricket Stadium**: 6.5 Km (~12 mins)
- **Gomti Riverfront Park & Marine Drive**: 3.5 Km (~8 mins)
- **Phoenix Palassio Shopping Mall**: 4.5 Km (~10 mins)

---

*© 2026 Hotel Dayal Paradise Lucknow. All rights reserved.*  
*Crafted with authentic Awadhi Tehzeeb and modern digital craftsmanship.*
