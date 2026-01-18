# TRACK 1: BUILDING THE HOUSE
## Complete Guide to Creating Your UG Math Tools Website Shell
## Version 1.0 - January 17, 2025

---

## 🎯 MISSION: Build the Professional Landing Page & Structure

**What we're building:** A clean, working website at `ugmathtools.com` with:
- Professional landing page
- Navigation structure
- Basic pages (About, Contact, etc.)
- Ready to receive modules later

**What we're NOT building (yet):**
- ❌ No games/modules
- ❌ No competition system
- ❌ No Firebase/backend
- ❌ No complex features

**Think of it like:** Building a beautiful house with empty rooms. Later we'll furnish the rooms (add games).

---

## 📐 TABLE OF CONTENTS

1. [What The Final Website Will Look Like](#1-what-the-final-website-will-look-like)
2. [Technical Setup (Step by Step)](#2-technical-setup-step-by-step)
3. [Repository Structure](#3-repository-structure)
4. [Landing Page Design](#4-landing-page-design)
5. [Navigation & Routing](#5-navigation--routing)
6. [Styling & Branding](#6-styling--branding)
7. [Deployment to Vercel](#7-deployment-to-vercel)
8. [Connecting Your Domain](#8-connecting-your-domain)
9. [Testing Checklist](#9-testing-checklist)
10. [Next Steps After Track 1](#10-next-steps-after-track-1)

---

## 1. WHAT THE FINAL WEBSITE WILL LOOK LIKE

### Homepage (ugmathtools.com)

```
┌─────────────────────────────────────────────────────────────┐
│  [UG MATH TOOLS Logo]            [About] [Modules] [Teacher]│
├─────────────────────────────────────────────────────────────┤
│                                                             │
│                    UG MATH TOOLS                            │
│              Underground Mathematics                        │
│                                                             │
│         Interactive Math Learning for Middle School        │
│                                                             │
│  ┌─────────────────────────────────────────────────────┐   │
│  │                                                     │   │
│  │  Transform your math classroom with engaging,      │   │
│  │  standards-aligned interactive modules.            │   │
│  │                                                     │   │
│  │  ✓ Gamified learning experiences                   │   │
│  │  ✓ Real-time teacher insights                      │   │
│  │  ✓ Individual & competitive modes                  │   │
│  │  ✓ North Carolina standards-aligned                │   │
│  │                                                     │   │
│  └─────────────────────────────────────────────────────┘   │
│                                                             │
│  ┌─────────────────┐      ┌─────────────────┐             │
│  │  FOR STUDENTS   │      │  FOR TEACHERS   │             │
│  │                 │      │                 │             │
│  │  • Practice     │      │  • Create games │             │
│  │    solo         │      │  • Track data   │             │
│  │  • Join games   │      │  • Assign work  │             │
│  │  • Track        │      │  • View reports │             │
│  │    progress     │      │                 │             │
│  │                 │      │                 │             │
│  │  [Get Started]  │      │  [Teacher Portal]│            │
│  └─────────────────┘      └─────────────────┘             │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  AVAILABLE MODULES                                          │
│                                                             │
│  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐    │
│  │ [Thumbnail]   │ │ [Thumbnail]   │ │ [Thumbnail]   │    │
│  │               │ │               │ │               │    │
│  │ Algebra       │ │ Multiplication│ │ Zombie        │    │
│  │ Expedition    │ │ Dojo          │ │ Apocalypse    │    │
│  │               │ │               │ │               │    │
│  │ Grades 6-8    │ │ Grades 3-6    │ │ Grades 6-8    │    │
│  │               │ │               │ │               │    │
│  │ [Coming Soon] │ │ [Coming Soon] │ │ [Coming Soon] │    │
│  └───────────────┘ └───────────────┘ └───────────────┘    │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  Built by a teacher, for teachers.                         │
│  Eastway Middle School • Charlotte, NC                     │
│                                                             │
│  © 2025 UG Math Tools                                      │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Navigation Structure

```
ugmathtools.com/                → Home (landing page)
ugmathtools.com/about           → About page
ugmathtools.com/modules         → Module catalog (list)
ugmathtools.com/teacher         → Teacher info page
ugmathtools.com/contact         → Contact/feedback form

[Future URLs - not built in Track 1:]
ugmathtools.com/solo/algebra    → Solo play (Track 2)
ugmathtools.com/compete         → Competition join (Track 2)
```

### Mobile View

```
┌──────────────────────┐
│ ☰  UG MATH TOOLS     │
├──────────────────────┤
│                      │
│   UG MATH TOOLS      │
│ Underground Math     │
│                      │
│ Interactive Learning │
│   for Middle School  │
│                      │
│  [FOR STUDENTS]      │
│  [FOR TEACHERS]      │
│                      │
│  Modules:            │
│  • Algebra Exp.      │
│  • Multiply Dojo     │
│  • Zombie Apoc.      │
│                      │
└──────────────────────┘
```

---

## 2. TECHNICAL SETUP (STEP BY STEP)

### Prerequisites Check

Before we start, verify you have:
- [x] GitHub account (you have this)
- [x] Domain purchased (ugmathtools.com) ✓
- [ ] Node.js installed on your computer
- [ ] Code editor (VS Code recommended)
- [ ] Vercel account

### Step 2.1: Install Node.js (If Not Already Installed)

**Check if you have it:**
1. Open Terminal (Mac) or Command Prompt (Windows)
2. Type: `node --version`
3. If you see a version number (like v18.0.0), skip to Step 2.2
4. If you get an error, continue below:

**Install Node.js:**
1. Go to https://nodejs.org/
2. Download the "LTS" version (left button)
3. Run the installer
4. Accept all defaults
5. Restart your computer
6. Open Terminal/Command Prompt again
7. Type: `node --version` to verify

### Step 2.2: Install VS Code (If You Don't Have It)

**Check if you have it:**
- Search your computer for "Visual Studio Code"
- If found, skip to Step 2.3

**Install VS Code:**
1. Go to https://code.visualstudio.com/
2. Download for your operating system
3. Install (accept defaults)
4. Open VS Code

### Step 2.3: Set Up Git (If Not Already Set Up)

**Check if configured:**
1. Open Terminal in VS Code (Terminal → New Terminal)
2. Type: `git config --global user.name`
3. If you see your name, skip to Step 2.4
4. If blank, continue:

**Configure Git:**
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Step 2.4: Create GitHub Repository

1. Go to github.com and log in
2. Click green "New" button
3. Fill out:
   - **Repository name:** `UGMathTools-Website`
   - **Description:** "Official UG Math Tools platform website"
   - **Visibility:** Private (for now)
   - **Initialize:** Check "Add a README file"
   - **Add .gitignore:** Select "Node"
4. Click "Create repository"

**Copy the repository URL:**
- Click the green "Code" button
- Copy the HTTPS URL (looks like: `https://github.com/yourusername/UGMathTools-Website.git`)

### Step 2.5: Clone Repository to Your Computer

**In VS Code:**
1. Press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows)
2. Type: "Git: Clone"
3. Paste your repository URL
4. Choose where to save it (I recommend: Documents/GitHub/)
5. Click "Open" when prompted

**Verify it worked:**
- You should see files in VS Code sidebar
- You should see a README.md file

---

## 3. REPOSITORY STRUCTURE

### The Folder Structure We'll Create

```
UGMathTools-Website/
├── public/                      # Static files
│   ├── index.html              # Main HTML file
│   ├── favicon.ico             # Website icon
│   └── assets/                 # Images, fonts, etc.
│       ├── logo.png
│       ├── hero-image.jpg
│       └── module-thumbnails/
│           ├── algebra.jpg
│           ├── multiply.jpg
│           └── zombie.jpg
│
├── src/                        # Source code
│   ├── main.jsx                # App entry point
│   ├── App.jsx                 # Main app component
│   │
│   ├── pages/                  # Page components
│   │   ├── Home.jsx            # Landing page
│   │   ├── About.jsx           # About page
│   │   ├── Modules.jsx         # Module catalog
│   │   ├── Teacher.jsx         # Teacher info
│   │   └── Contact.jsx         # Contact form
│   │
│   ├── components/             # Reusable components
│   │   ├── Header.jsx          # Top navigation
│   │   ├── Footer.jsx          # Bottom footer
│   │   ├── ModuleCard.jsx      # Module preview card
│   │   └── Hero.jsx            # Hero section
│   │
│   ├── styles/                 # CSS files
│   │   ├── index.css           # Global styles
│   │   ├── Home.css            # Page-specific styles
│   │   └── components.css      # Component styles
│   │
│   └── utils/                  # Helper functions
│       └── constants.js        # Site-wide constants
│
├── .gitignore                  # Git ignore file
├── package.json                # Dependencies
├── vite.config.js              # Build configuration
├── vercel.json                 # Deployment config
└── README.md                   # Documentation
```

### Step 3.1: Initialize React Project

**In VS Code Terminal:**

```bash
# Make sure you're in the project folder
cd UGMathTools-Website

# Create Vite + React project
npm create vite@latest . -- --template react

# When prompted:
# "Current directory is not empty. Remove existing files and continue? (y/N)"
# Type: y

# Install dependencies
npm install

# Install React Router for navigation
npm install react-router-dom

# Start development server to test
npm run dev
```

**What you should see:**
- Terminal shows: "Local: http://localhost:5173/"
- Open that URL in browser
- You should see default Vite + React page

**Press `Ctrl+C` in terminal to stop the server when done testing**

### Step 3.2: Create Folder Structure

**In VS Code, create these folders:**

1. Right-click `src` folder → New Folder → `pages`
2. Right-click `src` folder → New Folder → `components`
3. Right-click `src` folder → New Folder → `styles`
4. Right-click `src` folder → New Folder → `utils`
5. Right-click `public` folder → New Folder → `assets`
6. Right-click `assets` folder → New Folder → `module-thumbnails`

**Your `src` folder should now look like:**
```
src/
├── assets/         (came with Vite)
├── pages/          (you created)
├── components/     (you created)
├── styles/         (you created)
├── utils/          (you created)
├── App.jsx
├── App.css
├── main.jsx
└── index.css
```

---

## 4. LANDING PAGE DESIGN

### Design Decisions You Need to Make

Before we code the landing page, decide on these:

#### **Decision 1: Color Scheme**

**Option A: Professional Blue**
- Primary: #2563eb (blue)
- Secondary: #10b981 (green)
- Accent: #f59e0b (amber)
- Background: #f8fafc (light gray)

**Option B: Educational Purple**
- Primary: #7c3aed (purple)
- Secondary: #ec4899 (pink)
- Accent: #14b8a6 (teal)
- Background: #faf5ff (light purple)

**Option C: Energetic Orange**
- Primary: #ea580c (orange)
- Secondary: #0891b2 (cyan)
- Accent: #84cc16 (lime)
- Background: #fffbeb (cream)

**Your choice:** _________________

#### **Decision 2: Logo Approach**

**Option A: Text-only logo**
```
UG MATH TOOLS
Underground Mathematics
```

**Option B: Initials with tagline**
```
[UGM]
MATH TOOLS
```

**Option C: Custom design**
- Do you have a logo already?
- Should we create one using simple shapes?

**Your choice:** _________________

#### **Decision 3: Hero Section Content**

**What should the main headline say?**

Option A: "Transform Your Math Classroom"
Option B: "Interactive Math Learning That Works"
Option C: "Math Games Your Students Actually Want to Play"
Option D: Your own idea: _________________

**Your choice:** _________________

**What should the subheadline say?**

Option A: "Gamified, standards-aligned activities for middle school"
Option B: "Built by a teacher, for teachers"
Option C: "Engage students with real-time competitions and practice"
Option D: Your own idea: _________________

**Your choice:** _________________

#### **Decision 4: Call-to-Action Buttons**

**Primary button should say:**
- [ ] "Get Started"
- [ ] "Explore Modules"
- [ ] "Try It Free"
- [ ] Other: _________________

**Secondary button should say:**
- [ ] "For Teachers"
- [ ] "Teacher Portal"
- [ ] "Learn More"
- [ ] Other: _________________

#### **Decision 5: About Section**

**Should the landing page include info about you?**

- [ ] Yes, full bio (name, school, teaching experience)
- [ ] Yes, minimal (just "created by a 7th grade teacher")
- [ ] No, keep it generic/anonymous

**If yes, what should it say?**

_________________________________________________________________
_________________________________________________________________
_________________________________________________________________

#### **Decision 6: Module Showcase**

**How should modules be displayed on landing page?**

**Option A: Cards with thumbnails**
```
┌─────────────┐
│  [Image]    │
│             │
│ Module Name │
│ Description │
│ [Coming Soon]│
└─────────────┘
```

**Option B: List with icons**
```
🎮 Algebra Expedition - Solve equations in Dr. Martinez's adventure
📊 Multiplication Dojo - Master times tables with belt progression
🧟 Zombie Apocalypse - Calculate percentages to survive
```

**Option C: Featured module only**
```
FEATURED:
┌──────────────────────────────┐
│                              │
│  Algebra Expedition          │
│  [Large preview image]       │
│  37 levels • 6-8th grade     │
│                              │
│  [Learn More] [Play Solo]    │
└──────────────────────────────┘

+ View all modules →
```

**Your choice:** _________________

---

## 5. NAVIGATION & ROUTING

### Step 5.1: Set Up React Router

**Create `src/App.jsx`:**

```jsx
import { BrowserRouter as Router, Routes, Route } from 'react-router-dom';
import Header from './components/Header';
import Footer from './components/Footer';
import Home from './pages/Home';
import About from './pages/About';
import Modules from './pages/Modules';
import Teacher from './pages/Teacher';
import Contact from './pages/Contact';
import './styles/index.css';

function App() {
  return (
    <Router>
      <div className="app">
        <Header />
        <main className="main-content">
          <Routes>
            <Route path="/" element={<Home />} />
            <Route path="/about" element={<About />} />
            <Route path="/modules" element={<Modules />} />
            <Route path="/teacher" element={<Teacher />} />
            <Route path="/contact" element={<Contact />} />
          </Routes>
        </main>
        <Footer />
      </div>
    </Router>
  );
}

export default App;
```

### Step 5.2: Create Header Component

**Create `src/components/Header.jsx`:**

```jsx
import { Link } from 'react-router-dom';
import '../styles/components.css';

function Header() {
  return (
    <header className="header">
      <div className="header-container">
        <Link to="/" className="logo">
          <h1>UG MATH TOOLS</h1>
          <p className="tagline">Underground Mathematics</p>
        </Link>
        
        <nav className="nav">
          <Link to="/" className="nav-link">Home</Link>
          <Link to="/about" className="nav-link">About</Link>
          <Link to="/modules" className="nav-link">Modules</Link>
          <Link to="/teacher" className="nav-link">Teacher</Link>
          <Link to="/contact" className="nav-link">Contact</Link>
        </nav>

        {/* Mobile menu button - we'll add functionality later */}
        <button className="mobile-menu-btn">☰</button>
      </div>
    </header>
  );
}

export default Header;
```

### Step 5.3: Create Footer Component

**Create `src/components/Footer.jsx`:**

```jsx
import '../styles/components.css';

function Footer() {
  return (
    <footer className="footer">
      <div className="footer-container">
        <div className="footer-section">
          <h3>UG Math Tools</h3>
          <p>Interactive math learning for middle school</p>
        </div>
        
        <div className="footer-section">
          <h4>Quick Links</h4>
          <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
            <li><a href="/modules">Modules</a></li>
            <li><a href="/teacher">Teacher Portal</a></li>
          </ul>
        </div>
        
        <div className="footer-section">
          <h4>Contact</h4>
          <p>Eastway Middle School</p>
          <p>Charlotte, NC</p>
          <p><a href="/contact">Send Feedback</a></p>
        </div>
        
        <div className="footer-section">
          <p className="copyright">© 2025 UG Math Tools</p>
          <p className="attribution">Built by a teacher, for teachers</p>
        </div>
      </div>
    </footer>
  );
}

export default Footer;
```

---

## 6. STYLING & BRANDING

### Step 6.1: Global Styles

**Create/Edit `src/styles/index.css`:**

```css
/* ============================================
   GLOBAL STYLES & CSS VARIABLES
   ============================================ */

/* CSS Variables - CUSTOMIZE THESE BASED ON YOUR DESIGN DECISIONS */
:root {
  /* Colors - Update based on your chosen color scheme */
  --primary-color: #2563eb;      /* Main brand color */
  --secondary-color: #10b981;    /* Accent color */
  --accent-color: #f59e0b;       /* Highlight color */
  
  --text-primary: #1f2937;       /* Main text */
  --text-secondary: #6b7280;     /* Secondary text */
  --text-light: #9ca3af;         /* Muted text */
  
  --bg-primary: #ffffff;         /* Main background */
  --bg-secondary: #f8fafc;       /* Section backgrounds */
  --bg-dark: #1f2937;            /* Dark sections */
  
  /* Spacing */
  --spacing-xs: 0.5rem;
  --spacing-sm: 1rem;
  --spacing-md: 2rem;
  --spacing-lg: 4rem;
  --spacing-xl: 6rem;
  
  /* Typography */
  --font-primary: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
  --font-heading: 'Poppins', sans-serif;
  
  /* Border radius */
  --radius-sm: 0.375rem;
  --radius-md: 0.5rem;
  --radius-lg: 1rem;
  
  /* Shadows */
  --shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  --shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
}

/* Reset & Base Styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: var(--font-primary);
  color: var(--text-primary);
  background-color: var(--bg-primary);
  line-height: 1.6;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

h1, h2, h3, h4, h5, h6 {
  font-family: var(--font-heading);
  font-weight: 600;
  line-height: 1.2;
  color: var(--text-primary);
}

h1 { font-size: 3rem; }
h2 { font-size: 2.5rem; }
h3 { font-size: 2rem; }
h4 { font-size: 1.5rem; }

a {
  color: var(--primary-color);
  text-decoration: none;
  transition: color 0.2s ease;
}

a:hover {
  color: var(--secondary-color);
}

/* Layout */
.app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.main-content {
  flex: 1;
  width: 100%;
}

/* Container */
.container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 var(--spacing-md);
}

/* Buttons */
.btn {
  display: inline-block;
  padding: 0.75rem 1.5rem;
  border-radius: var(--radius-md);
  font-weight: 600;
  cursor: pointer;
  transition: all 0.2s ease;
  border: none;
  text-align: center;
}

.btn-primary {
  background-color: var(--primary-color);
  color: white;
}

.btn-primary:hover {
  background-color: var(--secondary-color);
  transform: translateY(-2px);
  box-shadow: var(--shadow-lg);
}

.btn-secondary {
  background-color: transparent;
  color: var(--primary-color);
  border: 2px solid var(--primary-color);
}

.btn-secondary:hover {
  background-color: var(--primary-color);
  color: white;
}

/* Utility Classes */
.text-center { text-align: center; }
.text-light { color: var(--text-light); }
.mt-1 { margin-top: var(--spacing-sm); }
.mt-2 { margin-top: var(--spacing-md); }
.mb-1 { margin-bottom: var(--spacing-sm); }
.mb-2 { margin-bottom: var(--spacing-md); }
```

### Step 6.2: Component Styles

**Create `src/styles/components.css`:**

```css
/* ============================================
   HEADER COMPONENT
   ============================================ */

.header {
  background-color: var(--bg-primary);
  border-bottom: 1px solid #e5e7eb;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: var(--shadow-sm);
}

.header-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  display: flex;
  flex-direction: column;
}

.logo h1 {
  font-size: 1.5rem;
  color: var(--primary-color);
  margin: 0;
}

.logo .tagline {
  font-size: 0.875rem;
  color: var(--text-secondary);
  margin: 0;
}

.nav {
  display: flex;
  gap: 2rem;
}

.nav-link {
  color: var(--text-primary);
  font-weight: 500;
  padding: 0.5rem 0;
  border-bottom: 2px solid transparent;
  transition: all 0.2s ease;
}

.nav-link:hover {
  color: var(--primary-color);
  border-bottom-color: var(--primary-color);
}

.mobile-menu-btn {
  display: none;
  background: none;
  border: none;
  font-size: 1.5rem;
  cursor: pointer;
  color: var(--text-primary);
}

/* Mobile Navigation */
@media (max-width: 768px) {
  .nav {
    display: none;
    /* We'll add mobile menu functionality later */
  }
  
  .mobile-menu-btn {
    display: block;
  }
}

/* ============================================
   FOOTER COMPONENT
   ============================================ */

.footer {
  background-color: var(--bg-dark);
  color: white;
  padding: var(--spacing-lg) 0 var(--spacing-md);
  margin-top: var(--spacing-xl);
}

.footer-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 2rem;
}

.footer-section h3 {
  color: white;
  margin-bottom: 1rem;
}

.footer-section h4 {
  color: var(--secondary-color);
  font-size: 1rem;
  margin-bottom: 0.5rem;
}

.footer-section p {
  color: #d1d5db;
  margin: 0.25rem 0;
}

.footer-section ul {
  list-style: none;
}

.footer-section ul li {
  margin: 0.5rem 0;
}

.footer-section a {
  color: #d1d5db;
}

.footer-section a:hover {
  color: var(--secondary-color);
}

.copyright {
  margin-top: 2rem;
  font-size: 0.875rem;
  color: #9ca3af;
}

.attribution {
  font-size: 0.875rem;
  color: #9ca3af;
  font-style: italic;
}
```

---

## 7. PAGE COMPONENTS

### Step 7.1: Home Page (Landing Page)

**Create `src/pages/Home.jsx`:**

```jsx
import '../styles/Home.css';

function Home() {
  return (
    <div className="home">
      {/* Hero Section */}
      <section className="hero">
        <div className="container">
          <div className="hero-content">
            <h1 className="hero-title">
              Transform Your Math Classroom
            </h1>
            <p className="hero-subtitle">
              Interactive, gamified math learning built by a teacher, for teachers.
              Engage students with real-time competitions and self-paced practice.
            </p>
            <div className="hero-buttons">
              <button className="btn btn-primary btn-lg">
                Explore Modules
              </button>
              <button className="btn btn-secondary btn-lg">
                Teacher Portal
              </button>
            </div>
          </div>
        </div>
      </section>

      {/* Features Section */}
      <section className="features">
        <div className="container">
          <h2 className="section-title">Why Teachers Love UG Math Tools</h2>
          
          <div className="feature-grid">
            <div className="feature-card">
              <div className="feature-icon">🎮</div>
              <h3>Gamified Learning</h3>
              <p>
                Students stay engaged with game-like experiences that make
                practicing math actually fun.
              </p>
            </div>
            
            <div className="feature-card">
              <div className="feature-icon">📊</div>
              <h3>Real-Time Insights</h3>
              <p>
                Track student progress live, identify struggles immediately,
                and download detailed analytics.
              </p>
            </div>
            
            <div className="feature-card">
              <div className="feature-icon">⚡</div>
              <h3>Two Modes</h3>
              <p>
                Solo practice for homework or team competitions for
                high-energy classroom activities.
              </p>
            </div>
            
            <div className="feature-card">
              <div className="feature-icon">✓</div>
              <h3>Standards-Aligned</h3>
              <p>
                All modules align with North Carolina math standards for
                middle school grades 6-8.
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* Modules Preview Section */}
      <section className="modules-preview">
        <div className="container">
          <h2 className="section-title">Available Modules</h2>
          
          <div className="module-grid">
            <div className="module-card">
              <div className="module-thumbnail">
                {/* Placeholder - replace with actual image */}
                <div className="placeholder-image">📐</div>
              </div>
              <h3>Algebra Expedition</h3>
              <p>Join Dr. Elena Martinez on an adventure solving equations</p>
              <span className="module-grade">Grades 6-8</span>
              <span className="module-status">Coming Soon</span>
            </div>
            
            <div className="module-card">
              <div className="module-thumbnail">
                <div className="placeholder-image">✖️</div>
              </div>
              <h3>Multiplication Dojo</h3>
              <p>Master times tables with belt progression system</p>
              <span className="module-grade">Grades 3-6</span>
              <span className="module-status">Coming Soon</span>
            </div>
            
            <div className="module-card">
              <div className="module-thumbnail">
                <div className="placeholder-image">🧟</div>
              </div>
              <h3>Zombie Apocalypse</h3>
              <p>Calculate percentages to survive the outbreak</p>
              <span className="module-grade">Grades 6-8</span>
              <span className="module-status">Coming Soon</span>
            </div>
          </div>
          
          <div className="text-center mt-2">
            <button className="btn btn-secondary">
              View All Modules
            </button>
          </div>
        </div>
      </section>

      {/* CTA Section */}
      <section className="cta-section">
        <div className="container">
          <h2>Ready to Transform Your Classroom?</h2>
          <p>Join hundreds of teachers using UG Math Tools</p>
          <button className="btn btn-primary btn-lg">
            Get Started Free
          </button>
        </div>
      </section>
    </div>
  );
}

export default Home;
```

**Create `src/styles/Home.css`:**

```css
/* ============================================
   HOME PAGE STYLES
   ============================================ */

/* Hero Section */
.hero {
  background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
  color: white;
  padding: var(--spacing-xl) 0;
  text-align: center;
}

.hero-content {
  max-width: 800px;
  margin: 0 auto;
}

.hero-title {
  font-size: 3.5rem;
  margin-bottom: 1.5rem;
  color: white;
}

.hero-subtitle {
  font-size: 1.25rem;
  margin-bottom: 2rem;
  color: rgba(255, 255, 255, 0.9);
  line-height: 1.8;
}

.hero-buttons {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}

.btn-lg {
  padding: 1rem 2rem;
  font-size: 1.125rem;
}

/* Features Section */
.features {
  padding: var(--spacing-xl) 0;
  background-color: var(--bg-secondary);
}

.section-title {
  text-align: center;
  margin-bottom: var(--spacing-lg);
  color: var(--text-primary);
}

.feature-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  margin-top: 3rem;
}

.feature-card {
  background: white;
  padding: 2rem;
  border-radius: var(--radius-lg);
  box-shadow: var(--shadow-md);
  text-align: center;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.feature-card:hover {
  transform: translateY(-5px);
  box-shadow: var(--shadow-lg);
}

.feature-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.feature-card h3 {
  color: var(--primary-color);
  margin-bottom: 1rem;
}

.feature-card p {
  color: var(--text-secondary);
  line-height: 1.6;
}

/* Modules Preview Section */
.modules-preview {
  padding: var(--spacing-xl) 0;
}

.module-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin-top: 3rem;
}

.module-card {
  background: white;
  border-radius: var(--radius-lg);
  overflow: hidden;
  box-shadow: var(--shadow-md);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.module-card:hover {
  transform: translateY(-5px);
  box-shadow: var(--shadow-lg);
}

.module-thumbnail {
  width: 100%;
  height: 200px;
  background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
  display: flex;
  align-items: center;
  justify-content: center;
}

.placeholder-image {
  font-size: 4rem;
}

.module-card h3 {
  padding: 1rem 1.5rem 0.5rem;
  color: var(--primary-color);
}

.module-card p {
  padding: 0 1.5rem;
  color: var(--text-secondary);
  margin-bottom: 1rem;
}

.module-grade {
  display: inline-block;
  padding: 0.25rem 0.75rem;
  background-color: var(--bg-secondary);
  border-radius: var(--radius-sm);
  font-size: 0.875rem;
  color: var(--text-secondary);
  margin: 0 1.5rem 1rem;
}

.module-status {
  display: inline-block;
  padding: 0.25rem 0.75rem;
  background-color: var(--accent-color);
  color: white;
  border-radius: var(--radius-sm);
  font-size: 0.875rem;
  margin: 0 1.5rem 1rem;
}

/* CTA Section */
.cta-section {
  background: linear-gradient(135deg, var(--bg-dark) 0%, var(--primary-color) 100%);
  color: white;
  padding: var(--spacing-xl) 0;
  text-align: center;
}

.cta-section h2 {
  color: white;
  margin-bottom: 1rem;
}

.cta-section p {
  font-size: 1.25rem;
  margin-bottom: 2rem;
  color: rgba(255, 255, 255, 0.9);
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-title {
    font-size: 2.5rem;
  }
  
  .hero-subtitle {
    font-size: 1rem;
  }
  
  .hero-buttons {
    flex-direction: column;
  }
  
  .feature-grid,
  .module-grid {
    grid-template-columns: 1fr;
  }
}
```

### Step 7.2: Create Placeholder Pages

**Create `src/pages/About.jsx`:**

```jsx
function About() {
  return (
    <div className="container" style={{padding: '4rem 2rem'}}>
      <h1>About UG Math Tools</h1>
      <p style={{marginTop: '1rem', lineHeight: '1.8', color: 'var(--text-secondary)'}}>
        UG Math Tools was created by a middle school math teacher in Charlotte, NC
        who wanted to make math more engaging for students. What started as simple
        practice worksheets evolved into a comprehensive platform of interactive,
        gamified learning experiences.
      </p>
      <p style={{marginTop: '1rem', lineHeight: '1.8', color: 'var(--text-secondary)'}}>
        Every module is designed with real classroom experience in mind, tested with
        actual students, and refined based on feedback from both students and teachers.
      </p>
      {/* Add more content later */}
    </div>
  );
}

export default About;
```

**Create `src/pages/Modules.jsx`:**

```jsx
function Modules() {
  return (
    <div className="container" style={{padding: '4rem 2rem'}}>
      <h1>All Modules</h1>
      <p style={{marginTop: '1rem', color: 'var(--text-secondary)'}}>
        Complete catalog coming soon. Check back as we migrate modules to the new platform.
      </p>
    </div>
  );
}

export default Modules;
```

**Create `src/pages/Teacher.jsx`:**

```jsx
function Teacher() {
  return (
    <div className="container" style={{padding: '4rem 2rem'}}>
      <h1>Teacher Portal</h1>
      <p style={{marginTop: '1rem', color: 'var(--text-secondary)'}}>
        Teacher features coming soon. You'll be able to create sessions, track student
        progress, and download detailed analytics.
      </p>
    </div>
  );
}

export default Teacher;
```

**Create `src/pages/Contact.jsx`:**

```jsx
function Contact() {
  return (
    <div className="container" style={{padding: '4rem 2rem'}}>
      <h1>Contact</h1>
      <p style={{marginTop: '1rem', color: 'var(--text-secondary)'}}>
        Have questions or feedback? Contact form coming soon.
      </p>
    </div>
  );
}

export default Contact;
```

---

## 8. DEPLOYMENT TO VERCEL

### Step 8.1: Create Vercel Account (If You Don't Have One)

1. Go to https://vercel.com/
2. Click "Sign Up"
3. Choose "Continue with GitHub"
4. Authorize Vercel to access your GitHub

### Step 8.2: Push Your Code to GitHub

**In VS Code Terminal:**

```bash
# Check status (see what files changed)
git status

# Add all files
git add .

# Commit with message
git commit -m "Initial website structure with landing page"

# Push to GitHub
git push origin main
```

**Verify on GitHub:**
- Go to your repository on GitHub
- You should see all your files there

### Step 8.3: Deploy to Vercel

1. Go to https://vercel.com/dashboard
2. Click "Add New" → "Project"
3. Find your `UGMathTools-Website` repository
4. Click "Import"
5. Configure project:
   - **Framework Preset:** Vite
   - **Root Directory:** ./
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
6. Click "Deploy"

**Wait 2-3 minutes for deployment to complete**

### Step 8.4: Test Your Deployed Site

1. Vercel will give you a URL like: `ugmathtools-website.vercel.app`
2. Click the URL to visit your site
3. Test all pages:
   - Home page loads ✓
   - Navigation works ✓
   - All pages accessible ✓
   - Mobile view looks okay ✓

---

## 9. CONNECTING YOUR DOMAIN

### Step 9.1: Add Domain in Vercel

1. In Vercel dashboard, go to your project
2. Click "Settings" tab
3. Click "Domains" in sidebar
4. Click "Add Domain"
5. Enter: `ugmathtools.com`
6. Click "Add"

**Vercel will show you DNS records to add**

### Step 9.2: Configure DNS at Namecheap

1. Log in to Namecheap
2. Go to "Domain List"
3. Click "Manage" next to ugmathtools.com
4. Click "Advanced DNS"
5. Add the records Vercel gave you:

**Typical setup (yours might vary slightly):**

| Type  | Host | Value                          | TTL       |
|-------|------|--------------------------------|-----------|
| A     | @    | 76.76.21.21                    | Automatic |
| CNAME | www  | cname.vercel-dns.com           | Automatic |

6. Save changes
7. Wait 10-60 minutes for DNS propagation

### Step 9.3: Verify Domain Connection

1. After waiting, go to https://ugmathtools.com
2. You should see your site!
3. Also test: https://www.ugmathtools.com

**If it doesn't work:**
- Wait longer (DNS can take up to 24 hours)
- Check DNS propagation: https://dnschecker.org/
- Verify records in Namecheap match Vercel exactly

---

## 10. TESTING CHECKLIST

Before considering Track 1 complete, test everything:

### Desktop Testing

- [ ] Landing page loads at ugmathtools.com
- [ ] Hero section displays correctly
- [ ] Features section visible
- [ ] Module cards display
- [ ] Header navigation works
- [ ] All nav links go to correct pages
- [ ] Footer displays
- [ ] Footer links work
- [ ] Colors match chosen scheme
- [ ] Text is readable
- [ ] Images load (if you added any)
- [ ] Buttons are clickable
- [ ] Hover effects work

### Mobile Testing

- [ ] Site loads on phone
- [ ] Text is readable (not too small)
- [ ] Buttons are tappable
- [ ] Navigation is accessible
- [ ] No horizontal scrolling
- [ ] Images fit screen
- [ ] Layout doesn't break

### Browser Testing

Test in at least these browsers:
- [ ] Chrome
- [ ] Safari
- [ ] Firefox
- [ ] Edge

### Performance Testing

- [ ] Page loads in under 3 seconds
- [ ] No console errors (F12 → Console)
- [ ] Smooth scrolling
- [ ] No lag when navigating

---

## 11. NEXT STEPS AFTER TRACK 1

### Immediate Improvements (Optional Polish)

**Week 1 Enhancements:**
- [ ] Add real logo (if you have one)
- [ ] Replace placeholder module thumbnails with actual images
- [ ] Add smooth scroll animations
- [ ] Improve mobile menu (hamburger functionality)
- [ ] Add favicon (browser tab icon)
- [ ] Add meta tags for SEO
- [ ] Add Google Analytics (if desired)

**Week 2 Content:**
- [ ] Write full About page content
- [ ] Create detailed module descriptions
- [ ] Add teacher testimonials (if you have any)
- [ ] Add screenshots of modules in action

### Moving to Track 2

Once you're satisfied with the website shell, we'll add:
1. Solo play mode for Algebra Expedition
2. Competition system
3. Teacher portal functionality

**But for now, Track 1 is complete when:**
✓ Professional landing page live at ugmathtools.com
✓ All navigation working
✓ Looks good on desktop and mobile
✓ You're proud to share it with colleagues

---

## 12. TROUBLESHOOTING COMMON ISSUES

### Issue 1: `npm run dev` doesn't work

**Symptoms:** Error message when starting development server

**Solutions:**
```bash
# Delete node_modules and reinstall
rm -rf node_modules
npm install

# Or try:
npm cache clean --force
npm install
```

### Issue 2: Page is blank/white screen

**Symptoms:** Nothing displays, just white screen

**Solutions:**
1. Check browser console (F12) for errors
2. Verify App.jsx is importing correctly
3. Check that all import paths are correct
4. Restart dev server (`Ctrl+C`, then `npm run dev` again)

### Issue 3: CSS not applying

**Symptoms:** Page shows content but no styling

**Solutions:**
1. Verify CSS files are imported in components
2. Check file paths are correct
3. Clear browser cache (Cmd+Shift+R / Ctrl+Shift+R)
4. Verify CSS variable names match

### Issue 4: Domain not working

**Symptoms:** ugmathtools.com shows error or old content

**Solutions:**
1. Wait longer (DNS takes time)
2. Check DNS records exactly match Vercel's requirements
3. Try incognito window (clears cache)
4. Check https://dnschecker.org/

### Issue 5: Build fails on Vercel

**Symptoms:** Deployment fails with error message

**Solutions:**
1. Check error log in Vercel dashboard
2. Verify package.json has all dependencies
3. Test local build: `npm run build`
4. Check Node.js version compatibility

---

## 13. GETTING HELP

### When You Need Help During Track 1

**In Our Chat:**
1. Describe what you're trying to do
2. Share the exact error message (if any)
3. Tell me what step you're on
4. Take a screenshot if helpful

**Example:**
> "I'm on Step 7.1, creating the Home page. When I save the file, I get this error in terminal: [paste error]. The page is blank. Here's a screenshot."

### Resources

**React Documentation:** https://react.dev/
**Vite Documentation:** https://vitejs.dev/
**CSS Reference:** https://developer.mozilla.org/en-US/docs/Web/CSS
**Vercel Documentation:** https://vercel.com/docs

---

## 14. CHECKLIST FOR MICHAEL

### Before Starting Track 1

- [ ] Master Plan uploaded to UGMathTools-Documentation repo
- [ ] Decided on color scheme
- [ ] Decided on logo approach
- [ ] Decided on headline text
- [ ] Decided on About section content
- [ ] Node.js installed
- [ ] VS Code installed
- [ ] Git configured
- [ ] Vercel account created

### During Track 1 (Work Sessions)

**Session 1: Setup & Structure (2 hours)**
- [ ] Create GitHub repo
- [ ] Initialize React project
- [ ] Create folder structure
- [ ] Set up routing
- [ ] Create Header/Footer components

**Session 2: Landing Page (2 hours)**
- [ ] Build Home page component
- [ ] Add hero section
- [ ] Add features section
- [ ] Add module preview section
- [ ] Style everything

**Session 3: Polish & Deploy (2 hours)**
- [ ] Create remaining pages (About, Modules, etc.)
- [ ] Test responsiveness
- [ ] Push to GitHub
- [ ] Deploy to Vercel
- [ ] Connect domain

**Session 4: Testing & Refinement (1 hour)**
- [ ] Test on multiple devices
- [ ] Fix any issues
- [ ] Add final touches
- [ ] Celebrate! 🎉

### After Track 1

- [ ] Update Master Plan (mark Track 1 complete)
- [ ] Take screenshots for documentation
- [ ] Share with 1-2 colleagues for feedback
- [ ] Plan Track 2 start date

---

## 15. WHAT SUCCESS LOOKS LIKE

### By End of Track 1, You Should Have:

**A Working Website:**
✓ Live at ugmathtools.com
✓ Professional landing page
✓ Clear navigation
✓ Responsive design (works on phones)
✓ Fast loading
✓ No errors

**Technical Foundation:**
✓ Clean GitHub repository
✓ Organized folder structure
✓ Reusable components
✓ Deployment pipeline working
✓ Easy to add new pages

**Confidence to:**
✓ Share URL with colleagues
✓ Show students where to find modules (once added)
✓ Make basic changes yourself
✓ Know how to deploy updates

**Ready for Track 2:**
✓ Structure in place to add modules
✓ Understanding of how pages are created
✓ Comfortable with the workflow

---

## 16. YOUR WORKING SCHEDULE

### Proposed Sessions (Adjust as Needed)

**Week 1:**
- Monday: Setup session (2 hours)
- Wednesday: Landing page session (2 hours)
- Friday: Check-in (30 min) - troubleshoot any issues

**Week 2:**
- Monday: Deploy session (2 hours)
- Wednesday: Testing & refinement (1 hour)
- Friday: Wrap-up & celebration (30 min)

**Total Time:** ~8-10 hours spread over 2 weeks

**Between Sessions:**
- You can work ahead if you want
- Or wait for our scheduled times
- Up to you!

---

**END OF TRACK 1 GUIDE**

---

This guide is your step-by-step manual for building the house. Keep it open while we work together. We'll go through each section at our own pace.

**Ready when you are, Michael. Let's build something great! 🚀**
