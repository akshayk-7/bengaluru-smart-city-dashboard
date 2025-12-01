## Bengaluru Smart City Dashboard

**Project Type**: Static Web UI (HTML + CSS only)  
**City**: Bengaluru (Bangalore)  
**Theme**: Smart City Command Center / Neon Dashboard

---

## Overview

This project is a **Smart City dashboard** for Bengaluru, built entirely with **HTML5 and CSS3** (no JavaScript).

It simulates a real command-center style interface that shows:

- Metro and BMTC status
- Traffic density at major junctions
- Weather, power outages, and smart electricity usage
- Emergency contacts, events, news, and a complaint form
- A CSS-only **Day / Night mode** toggle

You can use this as:

- A school/college **mini project**
- A **portfolio** UI piece
- A reference for **CSS Grid, Flexbox, and animations**

---

## Tech Stack

- **HTML5** – semantic layout with sections and panels
- **CSS3** – Grid, Flexbox, variables, gradients, animations
- **No JavaScript** – even the theme switch is pure CSS

Files:

- `index.html` – main dashboard page
- `styles.css` – all styling, themes, and animations

---

## How to Run

1. Make sure `index.html` and `styles.css` are in the **same folder**.
2. Open `index.html` in any modern browser:
   - Double-click `index.html`, or  
   - Right-click → **Open with** → Chrome / Edge / Firefox.

No server, no install, no build step required.

---

## Features

### Hero & Micro Stats

- Title: **Bengaluru Smart City Dashboard**
- Short explanation of what the dashboard shows
- Navigation: Home, Metro, Traffic, Weather, Alerts
- Rotating circular **logo** using CSS animation
- Micro-cards summarizing:
  - **Bengaluru Population** – 1.4 Crore  
  - **IT Companies** – 12,000+  
  - **Metro Lines** – 2 (expanding)

### Day / Night Theme Toggle (CSS Only)

- A hidden checkbox (`<input type="checkbox">`) plus a styled label acts as a switch.
- Theme colors are controlled with **CSS variables** (`--bg`, `--panel`, `--text`, etc.).
- **Light Mode** – White/blue, government-style dashboard.
- **Dark Mode** – Neon cyber-style dashboard with glowing cards.
- No JavaScript is used; everything is done using:

```css
#theme-toggle:checked + .app {
  /* override CSS variables for dark mode */
}
```

### Dashboard Panels

All panels are inside `<main class="dashboard">` as cards with the class `.panel`.

- **Weather Panel**
  - Static temperature (e.g. 27°C)
  - Areas: MG Road, Whitefield, Koramangala
  - CSS-only glowing sun icon

- **Power Outage Updates**
  - “No planned outages today”
  - Example entry: “JP Nagar · 2 PM – 4 PM · Planned maintenance”
  - Colored text for OK vs Warning states

- **BMTC Bus Routes**
  - Example routes: 500D, 600, KIA‑8
  - Realistic routes like “Kempegowda Bus Station → Hebbal → Whitefield”
  - Tags: **Frequent / Medium / Low frequency**
  - Static ETA labels

- **Metro Status**
  - Green, Purple, Airport lines
  - Status labels: Running / On Time / Delayed
  - Small **blinking CSS dots** for each line (metro signals)

- **Traffic Density**
  - Silk Board, KR Puram, Hebbal
  - Levels: High / Medium / Low
  - Styled like electronic boards

- **Emergency Services**
  - Hospital: 104  
  - Police: 100  
  - Fire: 101

- **City Systems (Animated Loaders)**
  - Energy Grid, Water Recycling, IoT Sensor Uptime
  - Uses animated CSS loading bars (no JS)

- **Smart Map**
  - Static map-style background image
  - Glowing blob overlay to simulate a city region

- **Smart Electricity Consumption**
  - Fake usage distribution:
    - Homes – 42%  
    - Industries – 30%  
    - IT Parks – 28%
  - Drawn with a **CSS bar chart** using custom properties and `::after`

- **City News (Auto Scroll)**
  - Metro extension, flood warnings, tech park news, smart parking
  - Vertical scrolling effect using `@keyframes news-scroll`

- **Smart Complaint System (UI Only)**
  - Fields:
    - Name
    - Location
    - Type of issue (Road, Water, Electricity, Public transport)
  - Submit button is **front-end only** (no backend)

- **Events & Highlights**
  - Tech Summit
  - Bengaluru Marathon
  - Metro expansion updates

---

## Design & Animation Notes

- **Layout**
  - CSS Grid for the overall dashboard layout
  - Flexbox inside many panels (e.g. metro list, bus cards)

- **Visual Style**
  - `Rajdhani` font for a techy, dashboard look
  - Gradients and glows for the hero and map
  - Rounded neon-style cards with hover lift effect

- **Animations**
  - Rotating logo circle (`@keyframes rotate`)
  - Blinking metro signals (`@keyframes blink`)
  - Animated loading bars (`@keyframes loading`)
  - Growing chart bars (`@keyframes grow`)
  - News auto-scroll (`@keyframes news-scroll`)

---

## How to Customize

- **Change city data**: Edit the relevant `<section class="panel ...">` blocks in `index.html`.
- **Change colors**: Tweak the CSS variables at the top of `styles.css` and inside the dark-mode block:

```css
:root {
  --bg: ...;
  --panel: ...;
  --neon: ...;
  --accent: ...;
  --text: ...;
  --muted: ...;
}

#theme-toggle:checked + .app {
  /* dark theme overrides */
}
```

- **Add/Remove panels**: Copy an existing `.panel` section in `index.html`, change the content and class name.

---

## Good Points to Mention in a Presentation

- Fully built with **only HTML and CSS** – no JavaScript at all.
- Uses **CSS Grid, Flexbox, animations, and variables**.
- Implements a **Day/Night mode** using the checkbox hack and CSS variables.
- Contains **fake yet realistic smart city data**: metro, BMTC, traffic, power, news, and more.
- Demonstrates both **UI design skills** and **front-end CSS skills**.


