武 WUSHU — Move by Move

A modern, interactive martial-arts learning page focused on Chinese martial arts, Wushu, Kung Fu, movement fundamentals, training, and daily practice.

The project presents martial-arts techniques one movement at a time, allowing users to select an art, browse individual movements, view visual references, read key technique points, and open demonstration videos.

✨ Features

Modern martial-arts themed design

Dark interface
Red and gold accent colors
Chinese-inspired typography and symbols
Responsive layout for desktop, tablet, and mobile

Martial arts library

Kung Fu
Wushu
Qinggong
Ruangong
Yinggong
Qigong
Neigong
Waigong
Shibaban Bingren

Move-by-move academy

Individual movement lessons
Movement descriptions
Key technical points
Previous/Next navigation
Progress indicator
Visual references
Links to YouTube demonstrations

Training foundation

Structure
Mobility
Technique
Conditioning
Awareness

Five-minute practice timer

5-minute default session
Start/pause functionality
Reset after completion
Selectable training focus

Responsive navigation

Desktop navigation
Mobile hamburger menu
Smooth scrolling between sections
🥋 Project Concept

The goal of WUSHU — Move by Move is to make martial-arts study easier to approach by breaking larger disciplines into smaller movements.

Instead of presenting an entire form or technique at once, the interface follows a simple learning progression:

See → Study → Practice → Repeat → Progress

The website is designed primarily as a visual learning and reference interface rather than a replacement for hands-on instruction.

📚 Included Sections
01 — Choose Your Path

Users can select a martial-art category from the main library.

Each category contains:

A Chinese character/symbol
A short description
A collection of movements
A button for opening the academy
02 — Move by Move

The academy dynamically loads the selected martial art.

Each movement contains:

Movement name
Description
Reference image
Key points
Demonstration link
Movement number
Progress indicator

The movement selector allows users to jump directly between lessons.

03 — Philosophy

A short philosophy section reinforces the project's learning approach:

See the movement.
Understand the structure.
Then make it your own.

04 — Foundation

The training section introduces five broad areas:

Structure
Mobility
Technique
Conditioning
Awareness

The idea is to establish physical fundamentals before progressing toward more difficult techniques.

05 — Daily Practice

The practice section provides a simple five-minute timer.

Users can select a training focus such as:

Horse stance
Qigong
Neigong
Waigong
Qinggong
Ruangong
Yinggong
Forms
Weapons
Feiyanzhoubi
Gaolaigaoqiludifeitengfa
🧩 Technical Structure

The project is currently implemented as a single HTML file containing:

HTML
├── Header
├── Hero
├── Martial Arts Library
├── Academy
├── Philosophy
├── Training Foundation
├── Daily Practice
└── Footer

CSS
├── Theme variables
├── Layout
├── Components
├── Responsive styles
└── Mobile navigation

JavaScript
├── Martial-arts data
├── Custom Web Components
├── Academy navigation
├── Movement rendering
└── Five-minute timer

🛠️ Technologies

The project uses standard web technologies:

HTML5
CSS3
Vanilla JavaScript
Web Components
CSS Grid
CSS Flexbox
Responsive media queries

No JavaScript framework or build system is required.

🧱 Custom Web Components

The interface uses native Web Components to keep repeated UI sections organized.

<site-header>

Creates the fixed navigation header and mobile menu.

<martial-arts>

Generates the martial-arts library from the arts JavaScript object.

<training-path>

Generates the five foundation-training cards.

<site-footer>

Creates the footer.

These components are registered with:

customElements.define()

📦 Martial Arts Data

The main content is stored inside the arts JavaScript object.

A simplified entry looks like:

"Kung Fu": {
  symbol: "拳",
  description: "Traditional Chinese martial-arts training.",
  moves: [
    {
      title: "Horse Stance — Ma Bu",
      image: "...",
      text: "A foundational stance...",
      points: [
        "Feet grounded",
        "Knees track with toes",
        "Chest relaxed"
      ],
      watch: "..."
    }
  ]
}


This makes it relatively easy to add new martial arts or movements without changing the academy interface.

▶️ Running the Project

Because the project does not require a build process, it can be opened directly in a browser.

Option 1 — Open the HTML file

Save the code as:

index.html


Then open it in a modern browser.

Option 2 — Use a local development server

For example, with VS Code and Live Server:

Open index.html
→ Start Live Server
→ Open the provided localhost address


A local server is recommended during development because the project loads external images and resources.

🌐 External Resources

The project currently references external resources for visual references and demonstration searches.

Images

Images are loaded from:

Wikimedia Commons
chinakungfu.net
Demonstrations

Movement buttons open YouTube search pages for relevant tutorials and demonstrations.

Because these resources are external, images or video results may change or become unavailable over time.

⚠️ Training & Safety

This website is intended as an educational and visual reference.

Martial-arts movements can involve physical risk, particularly:

Jumping techniques
Aerial movements
Weapons training
Impact conditioning
Advanced flexibility
Complex acrobatics
Partner training

Beginners should learn demanding techniques under the supervision of a qualified instructor and use appropriate training surfaces and equipment.

The site intentionally encourages gradual progression and emphasizes control, alignment, mobility, and safe landing mechanics.

🎨 Design System

The visual design uses a small set of CSS variables:

--bg: #080808;
--panel: #111;
--panel2: #181818;
--text: #f4f1e9;
--muted: #929292;
--red: #d84432;
--gold: #c8a45d;
--line: #292929;


The overall visual language combines:

Black backgrounds
Warm white typography
Red martial-arts accents
Gold labels
Large editorial-style headings
Chinese characters as decorative elements
Rounded panels
Subtle hover animations
📱 Responsive Design

The layout adapts at several breakpoints.

Desktop
Multi-column martial-arts cards
Two-column academy layout
Five-column foundation training layout
Full navigation
Tablet
Reduced card columns
Simplified training layout
Mobile
Hamburger navigation
Single-column academy layout
Single-column training section
Smaller image heights
Responsive typography
Horizontally scrollable movement selector
⏱️ Timer Logic

The daily practice timer starts at:

300


seconds, equivalent to five minutes.

The timer updates once per second using setInterval().

When it reaches zero, the timer stops and the control changes to a reset state.

🚀 Possible Future Improvements

Some useful additions for future versions include:

User progress tracking
Completed-movement indicators
LocalStorage support
Custom practice routines
Multiple timer durations
Search and filtering
Difficulty levels
Beginner/intermediate/advanced categories
More martial-arts systems
Embedded instructional videos
Instructor profiles
Audio guidance
Movement completion history
PWA/offline support
Better image attribution
Accessibility improvements
Keyboard navigation
Reduced-motion support
📄 Project Status

Status: Prototype / educational interface

The current version focuses on the frontend experience and interactive movement navigation. It does not include user accounts, a backend, databases, or persistent progress tracking.

🤝 Contributing

If you extend the project, consider keeping the movement data structure consistent.

For a new movement, provide:

{
  title: "Movement Name",
  image: "image-url",
  text: "Movement description.",
  points: [
    "Key point one",
    "Key point two",
    "Key point three"
  ],
  watch: "demonstration-url"
}


This allows the existing academy interface to render the new content automatically.

📜 License

Add the project's intended license here before publishing, such as MIT, Apache-2.0, or another license appropriate for your project.

Also verify the licensing and attribution requirements for every external image used by the website.

武 WUSHU

Train · Breathe · Move · Refine# wushu
# wushu
