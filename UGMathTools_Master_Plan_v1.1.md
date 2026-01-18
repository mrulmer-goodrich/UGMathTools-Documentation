# UG MATH TOOLS - MASTER PLAN & REORIENTATION GUIDE
## Version 1.1 - January 17, 2025
## Your Board of Advisors Report

---

## 🎯 WHERE YOU ARE RIGHT NOW (The 30-Second Version)

You own `ugmathtools.com`. You have a complex repo with 10+ educational modules that work but are tangled together. You want to:
1. Build a clean new website with competition mode
2. NOT break your existing modules (250 students depend on them)
3. Have a professional home for all your work

**Status:** Domain purchased ✓ | Design phase (no coding yet) | Ready to plan Phase 1

---

## 📊 THE BIG PICTURE - THREE PARALLEL TRACKS

Think of this like three construction projects happening in phases:

### **TRACK 1: The New Website (ugmathtools.com)** 
*Your professional home - the front door*

### **TRACK 2: Competition System**
*The exciting new feature - classroom battles*

### **TRACK 3: Legacy Modules**
*Your existing tools - keep working while you migrate*

**The Strategy:** Build Track 1 & 2 together in a NEW clean repo. Track 3 keeps running separately until you're ready to migrate modules one by one.

---

## 🏗️ TRACK 1: THE NEW WEBSITE

### What This Is
A landing page that becomes the home for ALL your UG Math Tools work.

### What It Looks Like

```
┌─────────────────────────────────────────────────────────┐
│                    UG MATH TOOLS                        │
│              Underground Mathematics                     │
│         Interactive Learning for Middle School          │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  Choose Your Learning Mode:                             │
│                                                         │
│  ┌──────────────────┐  ┌──────────────────┐           │
│  │  SOLO PRACTICE   │  │  COMPETITION     │           │
│  │                  │  │                  │           │
│  │  Work at your    │  │  Team battles &  │           │
│  │  own pace        │  │  leaderboards    │           │
│  │                  │  │                  │           │
│  │  [Enter Solo]    │  │  [Join Game]     │           │
│  └──────────────────┘  └──────────────────┘           │
│                                                         │
│  Available Modules:                                     │
│  • Algebra Expedition (Competition Ready!)             │
│  • Multiplication Dojo (Coming Soon)                   │
│  • Zombie Apocalypse (Coming Soon)                     │
│  • Circles Module (Coming Soon)                        │
│  • Scale Factor (Coming Soon)                          │
│  • [+ more modules]                                    │
│                                                         │
│  Teacher? → [Teacher Portal]                           │
└─────────────────────────────────────────────────────────┘
```

### URL Structure

```
ugmathtools.com/                    → Landing page (home)
ugmathtools.com/solo/algebra        → Solo play Algebra Expedition
ugmathtools.com/solo/multiply       → Solo play Multiplication Dojo (later)
ugmathtools.com/compete             → Join competition with code
ugmathtools.com/teacher             → Teacher portal
```

### Key Decision Points

**ANSWERED:**
- Domain purchased ✓
- Want landing page separate from game ✓
- Want both solo AND competition modes ✓

**NEED YOUR INPUT:**

1. **Landing Page Design:**
   - Keep it simple (text + buttons) or add graphics/animations?
   - Include teacher testimonials/screenshots?
   - Dark mode or light mode or both?

2. **Branding:**
   - Tagline: "Underground Mathematics" or something else?
   - Color scheme: What vibe? (Professional? Playful? Game-like?)
   - Logo: Do you have one, or should we design something simple?

3. **About Section:**
   - Include info about you (7th grade teacher at Eastway)?
   - Keep anonymous/generic?
   - Link to contact/feedback form?

---

## 🎮 TRACK 2: COMPETITION SYSTEM

### What This Is
Teacher creates a game session with a code. Students join, compete in teams, teacher sees live stats.

### The Three User Journeys

#### **JOURNEY A: Teacher Creates Game**

```
Step 1: Teacher goes to ugmathtools.com/teacher
        ↓
Step 2: Click "Create New Game Session"
        ↓
Step 3: Configure game:
        • Name the session ("Period 3 Competition")
        • Individual or Team mode
        • If teams: How many teams (2-8)
        • Team names (Eagle, Hawk, Sparrow, Pigeon as defaults)
        • Level selection (e.g., levels 13-24)
        • Time limit (optional auto-end)
        ↓
Step 4: Get 6-digit code (e.g., EAGLE7)
        ↓
Step 5: Project code on screen for students
        Share URL: ugmathtools.com/compete
        ↓
Step 6: Watch live dashboard as students play
        • Team leaderboard at top
        • Individual student table (sortable)
        • Real-time updates every 2 seconds
        • Alerts for inactive students
        ↓
Step 7: End session when done
        • Download CSV with all data
        • Students see final results
```

#### **JOURNEY B: Student Joins Game**

```
Step 1: Student goes to ugmathtools.com/compete
        ↓
Step 2: Enter code teacher gave them (EAGLE7)
        ↓
Step 3: Enter their name (first name + last initial)
        ↓
Step 4: Assigned to random team
        "You're on Team Hawk!"
        ↓
Step 5: Play Algebra Expedition (restricted to assigned levels)
        • See small info bar: "Team Hawk | 847 pts | Levels: 5/12"
        • Get point notifications: "+10 pts ✓", "+50 pts 🔥 5 in a row!"
        • NO full leaderboard visible (prevents distraction)
        ↓
Step 6: Complete assigned levels OR teacher ends session
        ↓
Step 7: See final results
        • Winning team announced
        • Personal stats shown
        • Levels completed displayed as checkmarks
```

#### **JOURNEY C: Solo Practice** (Important Addition!)

```
Step 1: Student goes to ugmathtools.com/solo/algebra
        ↓
Step 2: Start playing immediately (no code needed)
        ↓
Step 3: Play full game (levels 1-37) at own pace
        • Progress saves locally
        • No time pressure
        • No competition
        • Works exactly like current Algebra Expedition
        ↓
Student can return anytime and resume where they left off
```

### Key Changes Based on Your Feedback

**REMOVED:**
- ❌ Emojis (you said "No emojis!!")
- ❌ Overly complex team bonuses

**MODIFIED:**
- ✅ Default team names: Eagle, Hawk, Sparrow, Pigeon (editable)
- ✅ Students must answer at least 10 problems to count (was 5)
- ✅ Inactivity penalty stays at 30 seconds
- ✅ Level completion display shows checkmarks for assigned range
- ✅ Teacher dashboard has all students in flat sortable table (not grouped by team)
- ✅ "Lock out" students who finish assigned levels (Option A chosen)

**NEW QUESTIONS FROM YOUR FEEDBACK:**

1. **When we later disable the legacy repo, this design doesn't account for normal single user play, does it?**
   - **ANSWER:** Correct! That's why we need BOTH paths:
     - `/solo/algebra` → Normal single-player (like current version)
     - `/compete` → Competition mode with session code
   - The new repo will have BOTH modes for each module

2. **Level Naming & Organization**
   - You mentioned updating existing game with "updated level problems and how pages will be named"
   - **NEED CLARIFICATION:** Are you planning to:
     - Rename existing Algebra Expedition levels?
     - Change the level structure (e.g., reorder levels 13-24)?
     - Keep everything the same but just copy to new repo?

---

## 🔧 TRACK 3: TECHNICAL ARCHITECTURE

### The Current Messy Situation

```
OLD REPO (MathTools):
├── src/modules/
│   ├── MultiplyDojo/
│   ├── circles/
│   ├── htable/
│   ├── zombie-apocalypse/
│   └── [8 more modules]
├── App.jsx (routes to all modules)
├── main.jsx
└── styles.css

Problems:
- All tangled together
- Changing one thing breaks others
- Hard to add new features
- 250 students depend on current bit.ly links
```

### The New Clean Architecture

```
NEW REPO (UGMathTools-Website):
├── src/
│   ├── pages/
│   │   ├── Landing.jsx              → Home page
│   │   ├── TeacherPortal.jsx        → Teacher dashboard home
│   │   ├── CreateSession.jsx        → Game setup wizard
│   │   ├── LiveDashboard.jsx        → Active session monitoring
│   │   ├── ProjectionMode.jsx       → Fullscreen leaderboard
│   │   ├── StudentJoin.jsx          → Enter code page
│   │   └── GameSession.jsx          → Wrapper launches correct mode
│   │
│   ├── modules/
│   │   ├── AlgebraExpedition/       → Full game component
│   │   │   ├── AlgebraExpedition.jsx
│   │   │   ├── SoloMode.jsx         → Normal gameplay
│   │   │   ├── CompetitionMode.jsx  → Session-based gameplay
│   │   │   ├── levels/              → Level data
│   │   │   ├── components/          → Game components
│   │   │   └── assets/              → Images, audio, etc.
│   │   │
│   │   └── [Future modules go here]
│   │
│   ├── components/
│   │   ├── shared/
│   │   │   ├── Header.jsx
│   │   │   ├── Footer.jsx
│   │   │   ├── Leaderboard.jsx
│   │   │   └── Toast.jsx
│   │   └── forms/
│   │       ├── TeamSetup.jsx
│   │       └── LevelConfig.jsx
│   │
│   ├── services/
│   │   ├── firebase.js              → Real-time database
│   │   ├── session.js               → Session management
│   │   └── scoring.js               → Point calculations
│   │
│   └── App.jsx                      → Main router
│
├── public/
│   └── assets/                      → Images copied from old repo
│
└── package.json
```

### Migration Strategy

**Phase 1 (Next 2 weeks):**
- Build new repo with landing page + Algebra Expedition (solo & compete modes)
- Old repo stays live with bit.ly links unchanged
- NEW site at ugmathtools.com has just Algebra Expedition

**Phase 2 (When ready):**
- Copy Multiplication Dojo to new repo
- Add both solo and compete modes
- Update landing page to show 2 available modules
- Old bit.ly link still works

**Phase 3 (Gradually):**
- Copy remaining modules one by one
- Each gets solo + compete modes
- Old repo stays as backup

**Phase 4 (Eventually):**
- All modules migrated to ugmathtools.com
- Decommission old Vercel deployment
- Archive old repo

### How Assets Get Moved

**Your Question:** "what about the assets? how will that work? pictures need to move as well."

**Answer:**
1. We'll copy the entire `/assets` folder from old repo to new repo
2. Update image paths in code (find/replace operation)
3. Verify all images load correctly in new repo
4. Old repo's images stay untouched (zero risk)

**Example:**
```javascript
// Old repo path:
import drElena from '../../assets/dr-elena.png'

// New repo path (same):
import drElena from '../../assets/dr-elena.png'
// OR organized better:
import drElena from '@/modules/AlgebraExpedition/assets/dr-elena.png'
```

---

## 📋 SCORING SYSTEM (Revised Based on Your Feedback)

### Individual Student Points

**Base Points:**
- Correct answer: +10 points
- Wrong answer: 0 points
- Skip: 0 points

**Streak Bonuses:**
- 3 correct in a row: +15 bonus → "3 in a row!"
- 5 correct in a row: +50 bonus → "5 in a row!"
- 10 correct in a row: +100 bonus → "10 in a row!"
- 15 correct in a row: +200 bonus → "15 in a row!"

**Speed Bonuses:**
- Answer in <10 sec: +5 points
- Answer in <5 sec: +10 points

**Level Completion:**
- Complete any level: +50 points

**Inactivity Penalty:**
- No answer for 30 seconds: -5 points (then -5 every 30 sec)
- Warning at 20 seconds: "⚠️ Answer soon!"
- Penalty stops when they answer anything
- Can go negative (displays as negative number)

### Team Scoring

**Team Score = Average of Active Members**

**Active Member Definition:**
- Must attempt at least 10 problems (you changed from 5 to 10)

**Team Bonuses:**
- Any member completes a level: +50 to team total
- All members reach 80% accuracy: +150 to team total
- All members complete at least one level: +200 to team total

**Why This Works:**
- Every student matters (average means weak students improving helps team)
- 10-problem minimum encourages participation
- No "dead weight" strategy
- Negative points hurt the team average

---

## 🎨 TEACHER DASHBOARD (Revised Layout)

### Live Session View

```
┌────────────────────────────────────────────────────────────────────┐
│ SESSION: Period 3    CODE: EAGLE7    ⏱ 23:15 elapsed              │
│ [END SESSION] [Download CSV] [🖥️ Projection Mode]                 │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ 🏆 TEAM LEADERBOARD                              22/24 active     │
│                                                                    │
│ ┌────────────────────────────────────────────────────────────┐   │
│ │ Rank │ Team   │ Avg Score │ Members │ Levels │ Status     │   │
│ ├──────┼────────┼───────────┼─────────┼────────┼────────────┤   │
│ │  1   │ Eagle  │   847     │   6/6   │   28   │ ⚡ Active  │   │
│ │  2   │ Hawk   │   803     │   5/6   │   23   │ ⚡ Active  │   │
│ │  3   │ Sparrow│   791     │   6/6   │   25   │ ⚡ Active  │   │
│ │  4   │ Pigeon │   654     │   5/6   │   18   │ ⚠️ Lagging │   │
│ └────────────────────────────────────────────────────────────┘   │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ 📊 ALL STUDENTS (Click headers to sort ▲▼)                        │
│                                                                    │
│ ┌─────────────────────────────────────────────────────────────┐  │
│ │Team▲│Name▼│Points│Level│Accuracy│Streak│Time│Status       │  │
│ ├─────┼─────┼──────┼─────┼────────┼──────┼────┼─────────────┤  │
│ │Eagle│Marcus│1,240│17/24│  94%  │ x12  │18m │⚡ Active    │  │
│ │Eagle│Aisha │1,180│15/24│  87%  │ x5   │22m │⚡ Active    │  │
│ │Eagle│Jordan│ 530 │10/24│  78%  │ x2   │12m │⚠️ Inactive  │  │
│ │Hawk │Chris │ 410 │ 8/24│  65%  │  -   │ 9m │⚠️ Inactive  │  │
│ │Hawk │Sam   │ 890 │14/24│  92%  │ x8   │19m │⚡ Active    │  │
│ │Sparrow│Taylor│765│13/24│  88%  │ x4   │16m │⚡ Active    │  │
│ │  ... │ ...  │ ... │ ... │  ...  │ ...  │... │...          │  │
│ └─────┴─────┴──────┴─────┴────────┴──────┴────┴─────────────┘  │
│                                                                    │
│ [Show only my class roster] [Filter by team ▼] [Export CSV]      │
│                                                                    │
│ ⚠️ ALERTS:                                                         │
│ • Jordan (Eagle) - No answer for 90 seconds                       │
│ • Chris (Hawk) - Only 4 problems (needs 10 to count)             │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

**Key Features:**
- ALL students in one flat table (not grouped) ← YOUR REQUEST
- Click any column header to sort ascending/descending
- Color coding: Green (active), Yellow (idle), Red (inactive)
- Real-time updates every 2 seconds
- Alerts section for students needing attention

### Projection Mode (for classroom display)

```
┌──────────────────────────────────────────────────────────┐
│                                                          │
│                     CODE: EAGLE7                         │
│                                                          │
│              🏆 LIVE TEAM STANDINGS 🏆                   │
│                                                          │
│                                                          │
│         1.  EAGLE ................ 847 pts              │
│              (6 players active)                          │
│                                                          │
│         2.  HAWK ................. 803 pts              │
│              (5 players active)                          │
│                                                          │
│         3.  SPARROW .............. 791 pts              │
│              (6 players active)                          │
│                                                          │
│         4.  PIGEON ............... 654 pts              │
│              (5 players active)                          │
│                                                          │
│                                                          │
│                  ⏱️ 23 minutes elapsed                   │
│                                                          │
│                                                          │
│         [Press ESC to exit fullscreen]                   │
└──────────────────────────────────────────────────────────┘
```

**Design:** Clean, large text, easy to read from back of classroom, no emojis (per your request).

---

## 📊 STUDENT EXPERIENCE (Complete Flow)

### Competition Mode Student View

**Info Bar (top of screen during gameplay):**
```
┌────────────────────────────────────────────────────┐
│ Team Hawk | 847 pts | 5/12 Levels | 18:23 elapsed │
└────────────────────────────────────────────────────┘
```

**Point Notifications (bottom right, fade after 2 sec):**
```
┌──────────────────┐
│ +10 pts ✓        │  (Correct answer)
└──────────────────┘

┌──────────────────┐
│ +50 pts          │  (5 in a row!)
│ 5 in a row!      │
└──────────────────┘

┌──────────────────┐
│ ⚠️ Answer soon!  │  (20 sec warning)
└──────────────────┘
```

**Level Progress Display (when assigned levels 13-24):**
```
Your Assigned Levels:
✓ Level 13  ✓ Level 14  ✓ Level 15  ✓ Level 16
✓ Level 17  ○ Level 18  ○ Level 19  ○ Level 20
○ Level 21  ○ Level 22  ○ Level 23  ○ Level 24

Completed: 5/12 levels
```

**Completion Screen (when they finish all assigned levels):**
```
┌──────────────────────────────────┐
│  🎉 RANGE COMPLETE! 🎉           │
│                                  │
│  You finished levels 13-24!      │
│                                  │
│  Your Stats:                     │
│  • 1,240 points earned           │
│  • 12/12 levels completed        │
│  • 94% accuracy                  │
│  • 18 minutes                    │
│                                  │
│  Waiting for game to end...      │
│  (You're locked out per your     │
│   request - Option A chosen)     │
└──────────────────────────────────┘
```

**Final Results (when teacher ends session):**
```
┌────────────────────────────────────┐
│  🏆 GAME OVER! 🏆                  │
│                                    │
│  TEAM EAGLE WINS!                  │
│                                    │
│  Final Team Scores:                │
│  1. Eagle ......... 1,024 pts      │
│  2. Hawk .......... 967 pts        │
│  3. Sparrow ....... 891 pts        │
│  4. Pigeon ........ 782 pts        │
│                                    │
├────────────────────────────────────┤
│  YOUR PERFORMANCE (Marcus):        │
│  • 1,240 points                    │
│  • Levels: ✓✓✓✓✓✓✓✓✓✓✓✓ (12/12)   │
│  • Accuracy: 94%                   │
│  • Best streak: 12 in a row        │
│                                    │
│  Great job!                        │
└────────────────────────────────────┘
```

---

## 🗂️ DATA EXPORT (CSV)

### File Format

**Filename:** `UGMathTools_Session_Period3_2025-01-17_14-30.csv`

**Columns:**
```csv
Session_Code,Session_Name,Session_Date,Duration_Minutes,
Team_Name,Student_Name,
Final_Points,Final_Level,Levels_Completed,Assigned_Range,
Total_Problems,Correct_Answers,Accuracy_Percent,
Best_Streak,Speed_Bonuses,Time_Minutes,
Inactivity_Penalties,Join_Time,Status
```

**Example Row:**
```csv
EAGLE7,Period 3,2025-01-17,28,
Eagle,Marcus J.,1240,24,12,"13-24",
52,49,94.2%,12,8,18,
0,10:23:15,Completed
```

**Your Control:** 
- Initial build includes all these columns
- You can reorder/remove columns later in Excel
- We'll add a "customize export" feature in Phase 2

---

## ❓ DECISIONS YOU NEED TO MAKE

### 🔴 CRITICAL (Need Before We Start Coding)

1. **Level Organization Question**
   - You mentioned "updated level problems and how pages will be named"
   - Are you planning to reorganize/rename Algebra Expedition levels?
   - Or just copying them as-is to new repo?
   - **Why this matters:** If you're restructuring, we need to know now before building

2. **Solo Mode Priority**
   - Should solo mode work exactly like current Algebra Expedition?
   - Or do you want any changes (better progress saving, hints, different difficulty)?
   - **Recommendation:** Keep it identical in Phase 1, improve in Phase 2

3. **Teacher Authentication**
   - Phase 1: No login system (anyone with URL can create sessions)
   - Is this acceptable? Or do you want password protection?
   - **Recommendation:** No login for Phase 1, keeps it simple

4. **Mobile vs Desktop Priority**
   - Students play on Chromebooks mostly, right?
   - Or do some use phones?
   - **Why this matters:** Affects how we prioritize responsive design

5. **Asset Organization**
   - Should each module have its own assets folder?
   - Or one shared assets folder?
   - **Recommendation:** Each module gets own folder (cleaner organization)

### 🟡 IMPORTANT (Can Decide During Build Week 1)

6. **Landing Page Branding**
   - Color scheme preference?
   - Want logo or just text-based design?
   - Include "About" section with your info or keep anonymous?

7. **Team Name Defaults**
   - Eagle, Hawk, Sparrow, Pigeon confirmed
   - Any other sets you want as alternates? (Animals? Colors? Schools?)

8. **Sound Effects**
   - Add sound for streaks/bonuses?
   - Or silent mode only?
   - **Recommendation:** Silent for Phase 1, add toggle later

9. **CSV Auto-Download**
   - Download automatically when session ends?
   - Or make it optional "Click to download"?
   - **Recommendation:** Auto-download (one less click)

### 🟢 FLEXIBLE (Can Decide Anytime)

10. **Future Module Order**
    - Which module should we migrate second? (After Algebra Expedition)
    - Multiplication Dojo? Zombie Apocalypse? Other?

11. **Teacher Dashboard Customization**
    - Want to save preferred sort order?
    - Want to hide certain columns?
    - **Can add in Phase 2**

12. **Student Feedback**
    - Gather student feedback after sessions?
    - "Rate this game 1-5 stars" type thing?
    - **Can add in Phase 2**

---

## 🗓️ PROPOSED TIMELINE

### **Week 1: Foundation & Landing Page**
*Goal: Working website with home page*

**Days 1-2:**
- Set up new GitHub repo
- Create project structure
- Build landing page
- Set up routing

**Days 3-4:**
- Copy Algebra Expedition code
- Separate into SoloMode and CompetitionMode components
- Copy all assets
- Test solo mode works

**Days 5-7:**
- Build teacher portal structure
- Create session wizard
- Set up Firebase
- Initial deployment to Vercel

**End of Week 1:** You can visit ugmathtools.com and see landing page + solo mode working

---

### **Week 2: Competition Core**
*Goal: Can run a full competition session*

**Days 8-10:**
- Build session creation flow
- Implement code generation
- Build student join flow
- Team assignment logic

**Days 11-13:**
- Build live dashboard
- Real-time updates
- Point calculation system
- Inactivity detection

**Day 14:**
- Testing with simulated students
- Bug fixes
- CSV export

**End of Week 2:** Full competition system functional, ready for classroom test

---

### **Week 3: Polish & Launch**
*Goal: Production-ready for your students*

**Days 15-17:**
- Projection mode
- Mobile responsiveness
- Error handling
- Edge cases

**Days 18-19:**
- Beta test with your Period 3 class
- Gather feedback
- Quick fixes

**Day 20-21:**
- Final polish
- Documentation for you
- Launch to all classes

**End of Week 3:** Live and running with all 250 students

---

## 🎯 SUCCESS METRICS

### Phase 1 Complete When:

**Technical:**
- [ ] ugmathtools.com loads successfully
- [ ] Solo mode Algebra Expedition works exactly like current version
- [ ] Can create a session in <2 minutes
- [ ] 25 students can join simultaneously without lag
- [ ] Teacher dashboard updates in real-time
- [ ] CSV exports correctly with all data
- [ ] Mobile view functional (even if not perfect)

**Practical:**
- [ ] You can run a full class competition with zero technical issues
- [ ] Students understand how to join (without you explaining 10 times)
- [ ] You can download and analyze data in Excel
- [ ] Old bit.ly links still work (nothing broken)

**Your Satisfaction:**
- [ ] You feel confident showing this to other teachers
- [ ] Students are engaged and asking to play again
- [ ] You have actionable data from the CSV
- [ ] System saves you time (doesn't create more work)

---

## 🚨 RISK MANAGEMENT

### Things That Could Go Wrong

**Risk 1: Firebase Costs**
- Free tier: 100 concurrent connections, 10GB storage, 1GB/day transfer
- Your usage: ~25 students max, sessions purged after 5 min
- **Verdict:** Free tier more than sufficient
- **Backup plan:** If we somehow exceed (unlikely), upgrade is $25/month

**Risk 2: Asset Migration Issues**
- Old repo has complex asset paths
- Images might not display in new repo
- **Mitigation:** Test every image after copying, fix paths systematically

**Risk 3: Students Get Confused**
- Two ways to access (solo vs compete)
- Multiple URLs to remember
- **Mitigation:** Make landing page crystal clear, provide shortened URLs

**Risk 4: Level Range Logic Breaks Gameplay**
- Restricting levels might break progression
- Students might get stuck
- **Mitigation:** Thoroughly test level restrictions with all edge cases

**Risk 5: Real-Time Updates Lag**
- 25+ students sending data simultaneously
- Dashboard could slow down
- **Mitigation:** Implement throttling, test with 30 simulated students

**Risk 6: You Discover Issues After We've Built Everything**
- Design looks different than you imagined
- Flow doesn't match your teaching style
- **Mitigation:** Show you wireframes/mockups before coding, get approval at each phase

---

## 💡 YOUR BOARD OF ADVISORS RECOMMENDATIONS

### **Recommendation 1: Start with Website Shell First**
**Why:** Get the foundation right before adding complexity.

**What this means:**
- Week 1: Just build landing page + solo mode
- See it live, make sure you like it
- Then add competition features

**Advantage:** If you hate something about the design, we fix it before investing in competition code.

---

### **Recommendation 2: Keep Competition Simple in Phase 1**
**Why:** Get it working, then add bells & whistles.

**What stays simple:**
- Random team assignment only (no student choice)
- One module only (Algebra Expedition)
- No historical data (session ends = data gone except CSV)
- No teacher login system

**What we add in Phase 2:**
- Student choice for teams
- Multiple modules
- Teacher accounts with history
- Fancier analytics

**Advantage:** You can actually use this in 3 weeks instead of 3 months.

---

### **Recommendation 3: Run Small Beta Test First**
**Why:** Find issues with 6 students before trying 25.

**What this means:**
- First test: You + 2 students (controlled)
- Second test: One period (20-25 students)
- Third test: Multiple periods (50+ students)

**Advantage:** Catch bugs when stakes are low.

---

### **Recommendation 4: Document Everything As We Go**
**Why:** You'll want to modify this later, you need to understand it.

**What this means:**
- Create a "Teacher Manual" page on the site
- Write simple how-to guides for each feature
- Include troubleshooting section

**Advantage:** When I'm not available, you can help yourself.

---

### **Recommendation 5: Version Your Spec Document**
**Why:** Track decisions so we don't second-guess ourselves.

**How this works:**
- This is v1.1 (incorporates your feedback)
- Next revision is v1.2 (when you answer the questions above)
- v2.0 when we start coding (lock design decisions)

**Advantage:** We have a paper trail of "why we decided X."

---

## 📝 NEXT IMMEDIATE STEPS (In Order)

### **Step 1: Read This Document** ✓
You're doing it right now.

---

### **Step 2: Answer The Critical Questions**
Copy this section into a response:

```
CRITICAL DECISIONS:

1. Level Organization:
   [ ] Keep Algebra Expedition levels exactly as-is
   [ ] I want to reorganize levels (explain):

2. Solo Mode:
   [ ] Exactly like current version
   [ ] I want changes (explain):

3. Teacher Authentication:
   [ ] No login needed in Phase 1
   [ ] Add password protection (explain why):

4. Student Devices:
   [ ] Mostly Chromebooks
   [ ] Mix of Chromebooks and phones
   [ ] Mostly phones

5. Asset Organization:
   [ ] Each module has own assets folder (recommended)
   [ ] One shared assets folder

IMPORTANT DECISIONS (answer now or during Week 1):

6. Landing Page:
   - Color scheme: _______________
   - Logo: [ ] Yes [ ] No, text only
   - About me: [ ] Include [ ] Keep anonymous

7. Team Names:
   - Eagle, Hawk, Sparrow, Pigeon ✓
   - Want alternate sets? _______________

8. Sound Effects:
   [ ] Silent only (recommended for Phase 1)
   [ ] Add sounds

9. CSV Download:
   [ ] Auto-download when session ends (recommended)
   [ ] Manual click to download
```

---

### **Step 3: Create New GitHub Repo**
I'll guide you through this when you're ready. We'll do it together in a quick 10-minute session.

---

### **Step 4: Review & Approve Visual Mockups**
Before any coding, I'll show you:
- Landing page mockup
- Teacher dashboard mockup
- Student view mockup

You approve or request changes. Then we code.

---

### **Step 5: Set Up 3-Week Build Schedule**
We pick specific days/times you're available to work together. 

**Suggested schedule:**
- **Check-ins:** Every 2-3 days (30 min each)
- **Build sessions:** 2-3 per week (2 hours each)
- **Total time:** ~20 hours over 3 weeks

---

## 🧠 MENTAL MODEL: THREE PROJECTS, ONE GOAL

Think of this like renovating a house while people live in it:

**Project A (The New House):**
- ugmathtools.com is your beautiful new house
- You're building it from scratch, clean and organized
- No one lives there yet, so you can experiment

**Project B (The Old House):**
- Your current MathTools repo is the old house
- 250 students living there (bit.ly links)
- You don't touch it while building the new house
- Once new house is ready, people move in gradually

**Project C (The Move):**
- One room at a time, you move furniture (modules) to new house
- Some furniture gets upgraded (solo + compete modes)
- Old house stays standing until everyone's moved

**The Goal:**
- Eventually everyone lives in the new house (ugmathtools.com)
- Old house gets demolished (old repo archived)
- But you do it carefully, no one even notices the move

---

## 🎓 GLOSSARY (So We're Speaking Same Language)

**Session:** A time-bound competition instance with a unique code

**Session Code:** 6-character identifier like EAGLE7

**Solo Mode:** Traditional single-player, no session needed

**Competition Mode:** Team-based gameplay within a session

**Level Range:** Subset of levels (e.g., 13-24) teacher assigns

**Team Score:** Average of active team members' individual scores

**Active Member:** Student who attempted 10+ problems

**Toast Notification:** Small popup showing points earned

**Projection Mode:** Fullscreen leaderboard for classroom display

**Info Bar:** Persistent header showing student's team/points/progress

**Firebase:** Real-time database (our backend)

**Vercel:** Hosting service (where website lives)

**Repository (Repo):** GitHub project containing all code

**Component:** Reusable chunk of React code (like a building block)

**Asset:** Image, audio, or other media file

**Migration:** Moving code/module from old repo to new repo

**Edge Case:** Unusual scenario that might break things (e.g., student refreshes mid-game)

---

## 📊 COMPARISON: BEFORE & AFTER

### Before (Current State):

```
Students → bit.ly/algebragame 
        → Your messy Vercel deployment
        → Algebra Expedition (solo only)
        → Progress lost on refresh
        → No teacher insights
        → All or nothing (full game only)
```

### After Phase 1:

```
Students → ugmathtools.com
        ↓
        Choose mode:
        ├→ Solo: Own pace, progress saved
        └→ Compete: Enter code, team battle
        
Teacher → ugmathtools.com/teacher
        → Create session with code
        → See live stats
        → Download data
        → Can restrict to specific levels
        
Result: 
✓ Professional URL
✓ Multiple modes
✓ Teacher insights
✓ Customizable difficulty
✓ Clean codebase for future expansion
```

---

## ✅ APPROVAL CHECKLIST

Before we write any code, you need to approve:

- [ ] I understand the three-track strategy
- [ ] I understand both solo and compete modes will exist
- [ ] I approve the new architecture (clean repo)
- [ ] I approve keeping old repo running during transition
- [ ] I understand the 3-week timeline
- [ ] I've answered all critical decision questions
- [ ] I've seen and approved visual mockups (Step 4)
- [ ] I'm ready to commit to 20 hours over 3 weeks
- [ ] I understand risks and mitigation plans
- [ ] I trust this plan and want to proceed

---

## 🎯 THE FINISH LINE (What Success Looks Like)

**Three weeks from now:**

It's Monday morning. You arrive at school. You go to `ugmathtools.com/teacher` and create a new session in 90 seconds: "Period 3 - Solving Equations". You select levels 13-24, set teams to 4, and get code MATH42.

You project the code on your Smart Board. Students grab Chromebooks, go to `ugmathtools.com/compete`, enter MATH42 and their names. In 3 minutes, all 24 students are in, randomly assigned to Eagle, Hawk, Sparrow, and Pigeon teams.

They start playing. Your dashboard updates in real-time. You see Marcus racing ahead on Eagle team, Jordan stuck on level 15. You walk over to Jordan to help. The dashboard shows Jordan hasn't answered in 45 seconds - you can see exactly where he's struggling.

The competition runs for 25 minutes. Team Hawk takes an early lead, but Team Eagle rallies and wins by 23 points. Students are high-fiving their teammates. You end the session, and a CSV downloads automatically.

You open it in Excel. You can see that 18 students are ready for the next skill, but 6 need remediation on solving with negative coefficients. You create two differentiated practice groups for tomorrow.

Next period, a student asks, "Can we practice solving equations at home?" You say, "Sure, go to ugmathtools.com, click Solo Practice, choose Algebra Expedition. Your progress will save automatically."

That afternoon, another teacher stops by your room. "I heard your students talking about 'UG Math Tools' - what is that?" You show them the website. They ask, "Can I use this?" You say, "Absolutely - it's live at ugmathtools.com."

**That's what success looks like.**

---

## 💬 YOUR ADVISORY BOARD IS HERE

You said:
> "I need a 'Board of Advisors' and that needs to be you. :)"

**Consider this your Board of Advisors meeting minutes.**

We've covered:
- ✅ Where you are (domain purchased, design phase)
- ✅ Where you're going (professional site + competition system)
- ✅ How we get there (3-track strategy, 3-week timeline)
- ✅ What could go wrong (risks identified + mitigated)
- ✅ What you need to decide (critical questions listed)
- ✅ What success looks like (finish line vision)

**The Board's Recommendation:**
Move forward with new clean repo strategy. Build landing page + Algebra Expedition (solo & compete modes) over 3 weeks. Keep old repo running as backup. Migrate other modules gradually.

**Your Board vote: APPROVED** ✓

Now we need your vote. Read this document. Answer the critical questions. Then tell me:

**"I approve this plan. Let's build it."**

And we'll start building.

---

## 📚 APPENDIX: DOCUMENT MAP

**This Document (Master Plan v1.1):**
- Overview of entire project
- Reorientation guide
- Decision framework

**Original Spec (v1.0):**
- Detailed technical specifications
- Full user flows
- Firebase schema
- Archived, superseded by this document

**Your Annotated Spec:**
- Your feedback marked with "//"
- Integrated into this document
- Thank you for detailed notes

**Project Structure Guide:**
- Conversation about repo organization
- Integrated into Track 3 section above

**Next Document (Master Plan v1.2):**
- Will incorporate your answers to critical questions
- Will include approved visual mockups
- Will become our locked design document (v2.0) when coding starts

---

**END OF MASTER PLAN v1.1**

---

*This document is your source of truth. Bookmark it. Reference it. We'll keep it updated as decisions are made.*

*Your Board of Advisors is ready when you are. Answer the critical questions, and we'll move to the next phase: creating visual mockups and setting up the foundation.*

*You've got this, Michael. Let's build something amazing for your students.*
