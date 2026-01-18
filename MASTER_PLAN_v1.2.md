# UG MATH TOOLS - MASTER PLAN v1.2
## Your One Living Document
## Updated: January 17, 2025

---

## 🎯 WHO YOU ARE

**Name:** Michael
**Job:** 7th grade math teacher, Eastway Middle School, Charlotte, NC
**Students:** 80 students (yours) | 250 students (all 7th grade) | 800 students (whole school)
**Skill Level:** Brilliant educator, coding beginner, learns by doing
**Work Style:** Copy code → paste in GitHub → deploy Vercel → test live site → repeat
**Tools:** GitHub (browser), Vercel, school Chromebook OR personal Mac
**Superpower:** Big picture thinking, sees the vision clearly
**Challenge:** Too much technical info = overwhelmed, needs baby steps

---

## 🏆 THE VISION (What You're Building)

**Phase 1 (Track 1): The Landing Page**
- Professional website at `ugmathtools.com`
- Landing page lists all your modules
- Click a module → Coming Soon (for now)
- Clean, simple, works on all devices

**Phase 2 (Track 2): Add First Module**
- Algebra Expedition available
- Two modes: Game Mode (progressive levels) | Practice Mode (pick any level)
- Solo play only (no competition yet)

**Phase 3 (Track 3): Competition System**
- Teachers create sessions with codes
- Students join, compete in teams
- Live leaderboards, data export

**Phase 4+: Add More Modules**
- Multiplication Dojo
- Proportional Tables
- Circles
- All other existing modules
- Each gets Game Mode + Practice Mode

---

## 📂 REPOSITORY STRUCTURE (DECIDED)

### **One Repo Strategy** ✓

**Repository Name:** `UGMathTools-Website`

**Why one repo?**
- One website = one repo
- Easier to manage
- Shared navigation/footer
- One deployment
- You can handle it

**Folder Structure:**
```
UGMathTools-Website/
├── README.md
├── package.json
├── public/
│   └── assets/           → Images, logos
├── src/
│   ├── main.jsx         → Entry point
│   ├── App.jsx          → Main router
│   ├── pages/
│   │   ├── Landing.jsx        → Module selector (home page)
│   │   ├── About.jsx          → About page
│   │   └── Contact.jsx        → Contact page
│   ├── components/
│   │   ├── Header.jsx         → Top navigation
│   │   ├── Footer.jsx         → Bottom footer
│   │   └── ModuleCard.jsx     → Module preview card
│   ├── modules/               → [Future: actual games go here]
│   │   ├── algebra-expedition/
│   │   ├── multiplication-dojo/
│   │   └── [others...]
│   └── styles/
│       └── index.css          → All styles
```

**Documentation Repo:** `UGMathTools-Documentation`
- Stores this Master Plan
- Stores design documents
- No code, just plans

---

## 🗺️ SITE MAP (What Pages Exist)

### **URLs:**
```
ugmathtools.com/                → Landing page (module selector)
ugmathtools.com/about           → About UG Math Tools
ugmathtools.com/contact         → Contact/feedback

[FUTURE - Not building yet:]
ugmathtools.com/play/algebra    → Algebra Expedition
ugmathtools.com/play/multiply   → Multiplication Dojo
ugmathtools.com/teacher         → Teacher portal
```

---

## 🎨 DESIGN DECISIONS

### **Landing Page Layout:**

```
┌─────────────────────────────────────────────┐
│  [Header: UG Math Tools logo + nav]         │
├─────────────────────────────────────────────┤
│                                             │
│          UG MATH TOOLS                      │
│      Interactive Math Learning              │
│       for Middle School                     │
│                                             │
│  ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                             │
│  Choose a Module:                           │
│                                             │
│  ┌─────────────┐  ┌─────────────┐          │
│  │ [Preview]   │  │ [Preview]   │          │
│  │             │  │             │          │
│  │ Algebra     │  │ Multiply    │          │
│  │ Expedition  │  │ Dojo        │          │
│  │             │  │             │          │
│  │ Coming Soon │  │ Coming Soon │          │
│  └─────────────┘  └─────────────┘          │
│                                             │
│  ┌─────────────┐  ┌─────────────┐          │
│  │ Proportional│  │ Circles     │          │
│  │ Tables      │  │ Module      │          │
│  │ Coming Soon │  │ Coming Soon │          │
│  └─────────────┘  └─────────────┘          │
│                                             │
├─────────────────────────────────────────────┤
│  [Footer: © 2025 UG Math Tools]            │
└─────────────────────────────────────────────┘
```

### **Color Scheme:** (You need to decide)
- [ ] Option A: Blue & Green (professional)
- [ ] Option B: Purple & Pink (educational)
- [ ] Option C: Orange & Cyan (energetic)

### **Logo:** (You need to decide)
- [ ] Text only: "UG MATH TOOLS"
- [ ] Have a logo image already
- [ ] Create simple logo later

---

## 💻 YOUR WORKFLOW (How You Actually Work)

### **Current Workflow:**
1. Edit code in GitHub (browser interface)
2. Commit changes
3. Vercel auto-deploys
4. Clear browser cache
5. Test live site
6. Repeat

### **NO Local Development** (That's Fine!)
- You don't run `npm run dev`
- You don't install Node.js
- You work directly in GitHub
- This is acceptable for now

### **Testing Environment:**
- School Chromebook (limited)
- Personal Mac (better for design work)
- Test on both to ensure compatibility

### **Concern About Mac vs PC:**
**SOLUTION:** Design with Tailwind CSS (responsive by default) or use relative units (%, rem) instead of fixed pixels. Test on both devices regularly.

---

## 🚀 TRACK 1: BUILDING THE LANDING PAGE

### **Goal:** 
Professional landing page at ugmathtools.com that lists all modules as "Coming Soon"

### **What We're Building:**
- ✓ Landing page with module cards
- ✓ Header with navigation
- ✓ Footer with info
- ✓ About page (simple placeholder)
- ✓ Contact page (simple placeholder)

### **What We're NOT Building Yet:**
- ❌ Actual modules/games
- ❌ Competition system
- ❌ Teacher portal
- ❌ User accounts

---

## 📋 STEP-BY-STEP INSTRUCTIONS (Start Here)

### **STEP 1: Set Up Documentation Repo** (5 minutes)

**Action:**
1. Go to github.com (log in)
2. Click green "New" button
3. Name: `UGMathTools-Documentation`
4. Description: "Planning documents for UG Math Tools"
5. Select: **Private**
6. Check: "Add a README file"
7. Click "Create repository"

**Verify:** You see your new repo with a README.md file

**Action:**
8. Click "Add file" → "Create new file"
9. Name it: `MASTER_PLAN.md`
10. Copy/paste this ENTIRE document into it
11. Scroll to bottom, click "Commit new file"

**Verify:** You see MASTER_PLAN.md in your repo

**Action:**
12. Copy the URL (looks like: `https://github.com/yourusername/UGMathTools-Documentation`)
13. Tell Claude: "My documentation repo is at [paste URL]"

**✓ Step 1 Complete When:** Claude can read your Master Plan live

---

### **STEP 2: Create Main Website Repo** (5 minutes)

**Action:**
1. Go to github.com
2. Click green "New" button
3. Name: `UGMathTools-Website`
4. Description: "Official UG Math Tools platform"
5. Select: **Private**
6. Check: "Add a README file"
7. Select: Add .gitignore: **Node**
8. Click "Create repository"

**Verify:** You see your new repo

**Action:**
9. Copy the URL
10. Tell Claude: "My website repo is at [paste URL]"

**✓ Step 2 Complete When:** Repo exists and you've shared URL with Claude

---

### **STEP 3: Initialize React Project** (10 minutes)

**PROBLEM:** You can't run commands locally on school computer.

**SOLUTION:** I'll give you a complete folder structure to upload.

**Action:**
1. Tell Claude: "I'm ready for Step 3. Give me the files."
2. Claude will provide a ZIP or individual files
3. You'll upload them to your GitHub repo

**Verify:** Repo has folders: `src/`, `public/`, and files like `package.json`

**✓ Step 3 Complete When:** Repo has proper React structure

---

### **STEP 4: Connect to Vercel** (5 minutes)

**Action:**
1. Go to vercel.com/dashboard
2. Click "Add New" → "Project"
3. Find `UGMathTools-Website`
4. Click "Import"
5. Settings:
   - Framework: **Vite**
   - Build Command: `npm run build`
   - Output Directory: `dist`
6. Click "Deploy"

**Verify:** After 2-3 minutes, Vercel gives you a URL like `ugmathtools-website.vercel.app`

**Action:**
7. Click the URL and visit it
8. You should see default React page

**✓ Step 4 Complete When:** Website deploys successfully

---

### **STEP 5: Build Landing Page** (Working Session with Claude)

**This is where we work together in real-time.**

**What will happen:**
1. I give you code for Landing.jsx
2. You create file in GitHub
3. Paste the code
4. Commit
5. Vercel auto-deploys
6. You test
7. We refine
8. Repeat

**Estimated time:** 2-3 hours

**✓ Step 5 Complete When:** Landing page looks good and shows module cards

---

### **STEP 6: Add Styling** (Working Session)

**What will happen:**
1. I give you CSS code
2. You paste into styles/index.css
3. Commit
4. Test colors, spacing, responsive design
5. Adjust until you love it

**Estimated time:** 1-2 hours

**✓ Step 6 Complete When:** Site looks professional and works on mobile

---

### **STEP 7: Connect Domain** (15 minutes)

**Action:**
1. In Vercel dashboard, go to your project
2. Settings → Domains
3. Add domain: `ugmathtools.com`
4. Vercel shows DNS records
5. Go to Namecheap → Domain List → Manage → Advanced DNS
6. Add the records Vercel gave you
7. Save
8. Wait 10-60 minutes

**Verify:** Visit ugmathtools.com → See your site!

**✓ Step 7 Complete When:** Your site loads at ugmathtools.com

---

## ✅ VERIFICATION CHECKLIST

### **Track 1 is Complete When:**

- [ ] ugmathtools.com loads successfully
- [ ] Landing page shows module cards
- [ ] "Coming Soon" displays on each module
- [ ] Header navigation exists
- [ ] Footer shows copyright
- [ ] About page accessible (even if basic)
- [ ] Contact page accessible (even if basic)
- [ ] Site works on phone (responsive)
- [ ] Site works on Chromebook
- [ ] Site works on Mac
- [ ] No console errors (F12 → Console tab)
- [ ] You're proud to share the URL

---

## 🎯 DECISIONS YOU NEED TO MAKE

### **Right Now (Before We Start Building):**

**Decision 1: Color Scheme**
- [ ] Blue & Green
- [ ] Purple & Pink  
- [ ] Orange & Cyan
- [ ] Other (describe): _______________

**Decision 2: Module List**
Which modules should appear on landing page?
1. Algebra Expedition ✓
2. Multiplication Dojo ✓
3. Proportional Tables ✓
4. Circles Module ✓
5. _______________________
6. _______________________
7. _______________________
8. _______________________

**Decision 3: About Page Content**
- [ ] Include your name and school
- [ ] Generic "created by a teacher" 
- [ ] Leave blank for now

---

## 📝 MODULE NAMING CONVENTIONS

### **In Code (folder names):**
```
algebra-expedition      (lowercase, hyphenated)
multiplication-dojo
proportional-tables
circles-module
```

### **Display Names (what users see):**
```
Algebra Expedition
Multiplication Dojo
Proportional Tables
Circles Module
```

### **URLs (future):**
```
ugmathtools.com/play/algebra-expedition
ugmathtools.com/play/multiplication-dojo
```

---

## 🔄 FUTURE MODULE STRUCTURE

When we add actual modules (Track 2+), each will have:

```
src/modules/algebra-expedition/
├── index.jsx              → Module entry point
├── GameMode.jsx           → Play levels progressively
├── PracticeMode.jsx       → Pick any level
├── levels/
│   ├── level-01.js        → Level data
│   ├── level-02.js
│   └── [etc...]
├── components/
│   ├── ProblemGenerator.jsx
│   └── LevelMap.jsx
├── assets/
│   ├── dr-elena.png
│   └── [other images]
└── styles.css
```

**But don't worry about this now.** This is Track 2.

---

## 💬 HOW TO WORK WITH CLAUDE

### **Starting a New Chat:**
"Hey Claude, check my Master Plan at [your GitHub URL]. We're working on [Topic] today."

### **When You're Stuck:**
"Claude, I'm on Step [X]. I did [action] and got [result]. Help?"

### **When You Need Code:**
"Claude, I'm ready for the code for [component name]."

### **When Something Breaks:**
"Claude, the site shows [error/problem]. What do I do?"

### **When You Want to Test:**
"Claude, I deployed. The site looks like [describe]. Is this right?"

---

## 🚨 IMPORTANT NOTES

### **About Mac vs PC/Chromebook:**
- Design on Mac (easier for you)
- Test on Chromebook regularly
- Use responsive design (works on all screens)
- Don't use pixel values (use %, rem, em)

### **About GitHub Workflow:**
- You work in browser ✓
- No need for local dev (for now)
- Vercel auto-deploys ✓
- This is fine for Track 1

### **About Vercel:**
- Free tier is plenty
- Unlimited deployments
- Auto-updates when you commit to GitHub
- Cache may need clearing (Cmd+Shift+R or Ctrl+Shift+R)

### **About Forgetting Things:**
- That's why this document exists
- Read only the section you're working on
- Come back when you need a reminder
- I'll always check this document before helping

---

## 📊 PROGRESS TRACKING

### **Track 1: Landing Page**
Status: Not Started

- [ ] Step 1: Documentation repo created
- [ ] Step 2: Website repo created  
- [ ] Step 3: React structure uploaded
- [ ] Step 4: Connected to Vercel
- [ ] Step 5: Landing page built
- [ ] Step 6: Styling complete
- [ ] Step 7: Domain connected

**Target:** Complete in 2-3 work sessions (6-8 hours total)

### **Track 2: First Module** 
Status: Not Started
(Details TBD)

### **Track 3: Competition System**
Status: Not Started
(Details TBD)

---

## 🎓 GLOSSARY (Terms You'll See)

**Repo:** Short for "repository" - where code lives on GitHub
**Component:** A piece of UI (like Header, Footer, ModuleCard)
**Deploy:** Pushing code to make it live on the internet
**Vercel:** Service that hosts your website
**React:** JavaScript framework for building websites
**Vite:** Tool that bundles React code for deployment
**Commit:** Saving changes in Git
**npm:** Package manager (installs code libraries)
**node_modules:** Folder with installed libraries (don't edit)
**public:** Folder for images, icons, static files
**src:** Folder for your code

---

## 📞 HELP & RESOURCES

### **When You're Totally Lost:**
1. Check this document (find the section you're on)
2. Ask Claude (reference the step number)
3. Take a screenshot if helpful

### **When Code Doesn't Work:**
1. Check for typos
2. Make sure file is in correct folder
3. Clear browser cache
4. Check Vercel deployment log
5. Ask Claude with exact error message

### **When Design Looks Wrong:**
1. Test on different device
2. Clear cache
3. Check CSS is imported correctly
4. Ask Claude for help

---

## ✨ CELEBRATE MILESTONES

**When You Complete:**
- Step 1-2: You have repos set up! 🎉
- Step 3-4: Your site is live (even if basic)! 🚀
- Step 5-6: Your landing page looks professional! 💎
- Step 7: Your domain works! You have a real website! 🏆

**Each step is progress. You got this!**

---

**END OF MASTER PLAN v1.2**

Last Updated: January 17, 2025
Next Review: After Track 1 completion

---

## 📌 QUICK REFERENCE

**Your Repos:**
- Documentation: `https://github.com/[username]/UGMathTools-Documentation`
- Website: `https://github.com/[username]/UGMathTools-Website`

**Your Domain:** ugmathtools.com (purchased ✓)

**Your Vercel:** vercel.com/dashboard

**Current Focus:** Track 1 - Building Landing Page

**Next Step:** Create documentation repo, share URL with Claude

---

*This is your one living document. Everything important is here. When you're lost, come back to this. When we make decisions, this updates. You're doing great, Michael. Let's build this step by step.* 🚀
