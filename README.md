# FIFA World Cup 2026 Live Tournament Dashboard

A responsive, single-file web application built with clean HTML5, CSS3, and modern vanilla JavaScript designed for tournament coordinators to manage and display group stage phases, wildcard tie-breakers, and multi-stage knockout brackets[cite: 1, 2, 72].

## 📋 Table of Contents
- Features
- Project Architecture
- Key Functionalities
- Data Model
- UI Styling & Themes
- Installation & Usage

---

## ✨ Features

- Group Stage Tracker (Pool Phase): Dynamic evaluation of groups A through L with automatic calculation of matches played (MP), wins (W), draws (D), losses (L), goals for (GF), goals against (GA), goal difference (GD), and total points (Pts)[cite: 102, 148, 149, 150, 151, 152].
- Overall 3rd Place Teams Ranking Matrix: Automatically updates and reflects the 12 third-placed teams across all groups, filtering the top 8 wildcards moving on to the next phase with special styling[cite: 72, 73, 152, 153, 173].
- Complete Knockout Bracket System: Fully scalable views for the complete final tournament progression path: Round of 32, Round of 16, Quarter-Finals, Semi-Finals, and The Finals[cite: 74, 112].
- Participants Ranking Dataset Search: Live dataset search bar allowing instant filtering by country name or assigned group across all 48 qualified countries[cite: 75, 76, 78, 145].
- Automatic Dark Mode Integration: Seamless toggle behavior adapting to native operating system preferences (prefers-color-scheme: dark) with meticulously configured color palettes[cite: 4].

---

## 🏗️ Project Architecture

The application operates entirely on the client side inside a single standalone document for zero-latency execution.

- code.html / index.html: Consolidated HTML5 layout, CSS layouts, and core JS engine[cite: 1].

### Components
1. Header Zone: Custom responsive branding layout featuring the official FIFA 2026 asset badge metadata and custom application favicon tracking[cite: 65, 70].
2. Main Tab Navigation Layer: Controls view states between the Pool Phase, Final Bracket, and Participant Datasets[cite: 136, 137].
3. Sub-Navigation Component System: Populates dynamic group tags dynamically and separates individual knockout rounds[cite: 122, 123, 137, 138].

---

## ⚙️ Key Functionalities

### Dynamic View Toggling
Controlled via native JS logic loops avoiding large external library loads:
- switchMainTab(id, btn)
- switchSubTab(id, btn, targetClass)

### Filtering Architecture
The participant searching module utilizes substring matches mapped to live table redraw listeners:
- filterParticipantsTable()

---

## 📊 Data Model

The application comes pre-loaded with official structured tournament seeds:

### Participant Records Sample (excelParticipantsData)
Tracks up to 48 teams with group assignments, names, rankings, and structural details[cite: 78].

### Match Score Object Format (mymatchResults)
Tracks active matches using unique identifier references mapped against live DOM inputs[cite: 87].

---

## 🎨 UI Styling & Themes

The interface implements customizable CSS variables allowing effortless reconfiguration of global accent systems:

- Primary Accent: #1a365d (Light Mode) / #4299e1 (Dark Mode) [cite: 1, 4]
- Secondary Accent: #2b6cb0 (Light Mode) / #63b3ed (Dark Mode) [cite: 2, 5]
- Background Base: #f4f6f9 (Light Mode) / #0f172a (Dark Mode) [cite: 1, 4]
- Qualified Highlight: rgba(56, 161, 105, 0.08) (Light) / rgba(56, 161, 105, 0.2) (Dark) [cite: 3, 6]

---

## 🚀 Installation & Usage

1. Clone or Copy: Save the layout code file locally as an index webpage element (e.g., index.html).
2. Launch Project: Open the saved file inside any modern browser (Chrome, Edge, Firefox, or Safari) directly—no local dev server or npm packages required.
3. Deploy Anywhere: Ready to host statically on platforms like GitHub Pages, Vercel, or Netlify.
