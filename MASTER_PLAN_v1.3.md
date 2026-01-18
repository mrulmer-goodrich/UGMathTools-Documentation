# UG MATH TOOLS - MASTER PLAN v1.3
## Your One Living Document
## Updated: January 17, 2025 - 6:30 PM

---

## ✅ TRACK 1 COMPLETE! 

**Achievements:**
- ✓ Domain purchased: ugmathtools.com
- ✓ Documentation repo created: UGMathTools-Documentation
- ✓ Website repo created: UGMathTools-Website
- ✓ Clean folder structure established
- ✓ Landing page live and working
- ✓ Domain connected and verified
- ✓ Poppins font forced globally
- ✓ Professional site at https://ugmathtools.com

**Time invested:** ~4 hours
**Status:** 🎉 SUCCESS

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

**Key Constraint:** Maximum 8 human hours for Track 2 (migration + fixes)

---

## 🏆 THE VISION (Updated)

**What You're Building:**

A platform for YOUR STUDENTS to feel successful, master skills, and meet their individual needs through gamified interactive math modules.

**Phase 1 (Track 1): Landing Page** ✓ COMPLETE
- Professional website at ugmathtools.com
- Landing page lists all modules
- Clean, simple, works on all devices

**Phase 2 (Track 2): Algebra Expedition Migration** ← YOU ARE HERE
- Copy Algebra Expedition from old repo
- Fix 22 specific issues (organized below)
- Add Game Mode vs Practice Mode distinction
- Keep everything that already works

**Phase 3 (Track 3): Competition System**
- Teachers create sessions with codes
- Students join, compete in teams  
- Live leaderboards, data export

**Phase 4+: Add More Modules**
- Multiplication Dojo
- Proportional Tables
- Circles
- All other existing modules

---

## 📂 REPOSITORY STRUCTURE

### **Repo 1: Documentation** ✓
```
UGMathTools-Documentation/
├── MASTER_PLAN.md (this file)
└── [other planning docs]
```

### **Repo 2: Website** ✓
```
UGMathTools-Website/
├── src/
│   ├── pages/
│   │   ├── Landing.jsx ✓
│   │   ├── About.jsx ✓
│   │   └── Contact.jsx ✓
│   ├── components/
│   │   ├── Header.jsx ✓
│   │   └── Footer.jsx ✓
│   ├── modules/
│   │   └── algebra-expedition/ ← NEXT: Copy here
│   └── styles/
│       └── index.css ✓
```

### **Repo 3: Old MathTools** (Legacy)
```
https://github.com/mrulmer-goodrich/MathTools
└── src/algebra/ ← Source to copy from
```

---

## 🚀 TRACK 2: ALGEBRA EXPEDITION MIGRATION

### **STRATEGY: SURGICAL FIXES, NOT REBUILD**

**Why this approach:**
- ✅ Levels 1-24 tested by 100+ students and work great
- ✅ No regression risk
- ✅ Preserve what works
- ✅ Fix specific issues incrementally
- ✅ Test after each fix

**What we'll do:**
1. Copy entire Algebra Expedition AS-IS to new repo
2. Copy required assets
3. Test it works in new site
4. Fix issues one by one from Michael's list
5. Test continuously

---

## 📋 THE 22 ISSUES - ORGANIZED BY PRIORITY

### **TIER 1: CRITICAL FIXES (Do First - Required for Track 2 Complete)**

**Issue #1: Game Saves/Progress** ✓ WORKING
- Current: Saves locally, can close and return
- Action: Migrate AS-IS, verify still works
- Priority: HIGH (but already working)

**Issue #5: Levels 1-24 Work** ✓ WORKING
- Current: Tested by 100+ students, no complaints
- Action: Migrate AS-IS, verify still works
- Priority: HIGH (but already working)

**Issue #21: Game Mode vs Practice Mode** 🔴 NEEDS FIXING
- Current: Distinction unclear
- Desired: 
  - **Game Mode:** Progressive levels (1→2→3... must complete in order)
  - **Practice Mode:** Pick any level freely
- Action: Add mode selector, implement logic
- Priority: CRITICAL
- Time estimate: 2 hours

**Issue #6: Practice Page - 36 Levels** 🔴 NEEDS FIXING
- Current: Redesigned for 36 levels but not displayed correctly
- Action: Update practice page UI to show all 36 levels
- Priority: CRITICAL
- Time estimate: 1 hour

**Issue #11: Answer Shuffle Bug** 🔴 NEEDS FIXING
- Current: One level has final answer always in 1st position
- Action: Find level, fix shuffle logic
- Priority: CRITICAL (affects fairness)
- Time estimate: 30 minutes

**Issue #15: Alignment of Operations** 🔴 NEEDS FIXING
- Current: "+5 to both sides" not aligned with "-5" term
- Why critical: Student understanding depends on this
- Action: Fix CSS/layout for step-by-step feedback
- Priority: CRITICAL (pedagogy)
- Time estimate: 1 hour

**Tier 1 Total Time:** ~4.5 hours

---

### **TIER 2: UI POLISH (Do Second - After Track 2 Works)**

**Issue #2: Exit Button Styling** 🟡
- Current: Gross styling
- Action: Redesign button with better CSS
- Time estimate: 15 minutes

**Issue #3: Floating Icons Horizontal** 🟡
- Current: Default to vertical
- Desired: Horizontal default
- Note: Varying button sizes make it messy without redesign
- Action: Design horizontal layout OR accept vertical for now
- Time estimate: 30 minutes OR defer

**Issue #4: Container Padding** 🟡
- Current: Excess padding inside and outside
- Action: Reduce padding in container CSS
- Time estimate: 20 minutes

**Issue #7: Story Intro Consistency** 🟡
- Current: Varying container sizes for 4 intro pages
- Desired: Consistent sizes
- Also: Remove "Page 1 of 4" footer
- Action: Standardize story container CSS, remove pagination
- Time estimate: 30 minutes

**Issue #12: Feedback Modal Alignment** 🟡
- Current: Step-by-step doesn't line up correctly, top-left problem field display issues
- Action: Fix modal CSS/layout
- Time estimate: 45 minutes

**Issue #13: Progress Tracker** 🟡
- Current: Could be refined/reimagined
- Action: TBD (needs design decisions)
- Time estimate: 1 hour

**Issue #14: Font Sizes** 🟡
- Current: Problems and answer choices too small, details lost
- Action: Increase font sizes for readability
- Time estimate: 20 minutes

**Issue #20: Success Overlay Animation** 🟡
- Current: Works but could be better
- Action: Update animation/styling
- Time estimate: 30 minutes

**Tier 2 Total Time:** ~3.5 hours

---

### **TIER 3: CONTENT/DESIGN (Do Third - Separate Track)**

**Issue #8: LevelIntro Redesign** 🟢
- Current: Broken, defaults to backup, story scattered
- Desired: Central location for:
  - Story element (small narrative)
  - "Teach slide" (how to solve this type)
  - Associated skill
  - Rule/concept
  - All level metadata (except problems)
- Action: Create centralized level data structure, rebuild LevelIntro component
- Time estimate: 3 hours
- Status: DEFER to Track 2.5

**Issue #9: Problem Generators** 🟢
- Current: Working but big clunky files
- Action: Refactor for cleaner code (optional optimization)
- Time estimate: 4 hours
- Status: DEFER (working = don't touch yet)

**Issue #10: Level Names/Story** 🟢
- Current: Need reimagining
- Action: Rewrite narrative/naming for all 36 levels
- Time estimate: 4 hours (content creation)
- Status: DEFER to content sprint

**Issue #16: More Answer Choices** 🟢
- Current: Restricted to 4 choices
- Desired: Some levels should have more options
- Action: Update level configs, adjust UI
- Time estimate: 2 hours
- Status: DEFER

**Issue #17: Map Icon Replacement** 🟢
- Current: Map icon doesn't do much
- Desired: Show Mastery Levels and Mastery Bands quickly
- Note: Practice mode uses checkmarks per level
- Action: Design new visualization
- Time estimate: 2 hours
- Status: DEFER

**Issue #18: Stats Tracking (Today vs Lifetime)** 🟢
- Current: Saves forever locally
- Desired:
  - Separate today vs lifetime stats
  - Ability to clear each independently
  - Floating icon shows today only
- Action: Refactor stats storage structure
- Time estimate: 2 hours
- Status: DEFER to Track 2.5

**Issue #19: Distractor Verification** 🟢
- Current: Not all distractors verified as good
- Action: Review and improve wrong answer choices
- Time estimate: 6 hours (content work)
- Status: DEFER to content sprint

**Issue #22: File Structure** 🟢
- Current: Don't like it
- Action: Reorganize module folders
- Time estimate: 2 hours
- Status: DEFER (low priority)

**Tier 3 Total Time:** ~25 hours (DEFERRED)

---

## 🎯 TRACK 2 COMPLETION CRITERIA

**Track 2 is complete when:**

### **Must Have (Critical):**
- [ ] Algebra Expedition copied to new repo
- [ ] Levels 1-36 accessible
- [ ] Game Mode (progressive) works
- [ ] Practice Mode (pick any level) works
- [ ] Game saves/progress works
- [ ] Issue #11 fixed (answer shuffle)
- [ ] Issue #15 fixed (alignment)
- [ ] Deployed and tested by students

### **Should Have (Important):**
- [ ] Issue #6 fixed (36 levels display)
- [ ] Issue #2 fixed (exit button)
- [ ] Issue #14 fixed (font sizes)

### **Nice to Have (Polish):**
- [ ] Issue #4 fixed (padding)
- [ ] Issue #7 fixed (story consistency)
- [ ] Issue #12 fixed (feedback modal)

**Target Time:** 6-8 human hours
**Target Completion:** Next week

---

## 🔧 TRACK 2 STEP-BY-STEP PLAN

### **Phase 1: Copy & Verify (2 hours)**

**Step 1: Copy Algebra Folder**
- Copy entire `/src/algebra` from old repo to new repo
- Place at: `/src/modules/algebra-expedition/`
- Commit and deploy

**Step 2: Copy Assets**
- Identify which assets AE uses
- Copy to `/public/assets/algebra-expedition/`
- Update image paths in code

**Step 3: Integrate with Landing Page**
- Add route: `/play/algebra-expedition`
- Update Landing.jsx to link to it
- Test: Click module card → loads game

**Step 4: Verify Core Functionality**
- Test levels 1-24 work
- Test game saves/resumes
- Test problem generation
- Test feedback system

**Checkpoint:** If everything works, proceed. If broken, debug before continuing.

---

### **Phase 2: Critical Fixes (4 hours)**

**Fix #21: Game Mode vs Practice Mode**
- Create mode selector component
- Implement progressive logic (Game Mode)
- Implement free selection (Practice Mode)
- Test both modes

**Fix #6: Display 36 Levels**
- Update practice page grid
- Test scrolling/layout
- Verify all levels accessible

**Fix #11: Answer Shuffle**
- Find problematic level
- Fix shuffle algorithm
- Test multiple times

**Fix #15: Operation Alignment**
- Update step-by-step CSS
- Test with various problem types
- Verify student-facing clarity

**Checkpoint:** Critical functionality complete, students can use effectively.

---

### **Phase 3: Polish (1-2 hours)**

**Fix #2, #4, #14: Quick CSS fixes**
- Exit button styling
- Container padding
- Font size increases

**Test & Deploy**
- Test on Chromebook
- Test on phone
- Deploy to production
- Announce to students

**Checkpoint:** Track 2 complete! 🎉

---

## ✅ "FIX LATER" LIST

**Landing Page Content:**
- Change "built by a teacher, for teachers" to "built for students to feel successful and master skills"
- Update hero text to reflect student focus
- Add testimonials (optional)

**Header Design:**
- Implement collapsible header (shows on hover, hides when not)
- OR minimize header (reduced height, font, spacing)
- Goal: Maximize screen space

**Other UI Improvements:**
- Add favicon
- Add meta tags for SEO
- Improve mobile navigation

---

## 🗺️ FUTURE TRACKS (After Track 2)

### **Track 2.5: Content & Design Polish**
- LevelIntro redesign (Issue #8)
- Stats tracking overhaul (Issue #18)
- Level names/story rewrite (Issue #10)

### **Track 3: Competition System**
- Teacher portal
- Session creation
- Student join flow
- Team assignment
- Live leaderboards
- Data export (CSV)

### **Track 4: Additional Modules**
- Multiplication Dojo
- Proportional Tables
- Circles
- Zombie Apocalypse
- Vault Heist

---

## 💬 HOW TO WORK WITH CLAUDE

### **Starting a New Chat:**
"Hey Claude, check my Master Plan at [GitHub URL]. We're working on [specific issue] today."

### **When Starting Work:**
"Claude, I'm ready to work on Track 2, Phase 1. Let's start with Step 1."

### **When You're Stuck:**
"Claude, I'm on [step/issue]. I did [action] and got [result]. Help?"

### **When You Want to Skip Something:**
"Claude, let's defer Issue #[X] to later. Move to next critical issue."

---

## 📊 PROGRESS TRACKING

### **Track 1: Landing Page** ✅ COMPLETE
- [x] Documentation repo created
- [x] Website repo created  
- [x] React structure uploaded
- [x] Connected to Vercel
- [x] Landing page built
- [x] Styling complete
- [x] Domain connected
- [x] Poppins font forced globally

**Time Spent:** ~4 hours  
**Status:** 🎉 SUCCESS

---

### **Track 2: Algebra Expedition** 🏗️ IN PROGRESS
**Phase 1: Copy & Verify**
- [ ] Copy algebra folder
- [ ] Copy assets
- [ ] Integrate with landing page
- [ ] Verify core functionality

**Phase 2: Critical Fixes**
- [ ] Issue #21: Game vs Practice mode
- [ ] Issue #6: Display 36 levels
- [ ] Issue #11: Answer shuffle bug
- [ ] Issue #15: Operation alignment

**Phase 3: Polish**
- [ ] Issue #2: Exit button
- [ ] Issue #4: Padding
- [ ] Issue #14: Font sizes
- [ ] Final testing

**Time Budget:** 6-8 hours  
**Status:** ⏳ NOT STARTED

---

### **Track 3: Competition System** 📅 PLANNED
Status: Not started (after Track 2)

---

## 🚨 CONSTRAINTS & REMINDERS

### **Time Constraints:**
- Track 2 maximum: 8 human hours
- Work in focused 2-hour sessions
- Test after every major change
- Don't over-engineer

### **Quality Gates:**
- No regression (levels 1-24 must keep working)
- Student-tested before announcing
- Works on Chromebook (primary device)
- Mobile-friendly (secondary)

### **Working Style:**
- GitHub browser editing (no local dev needed)
- Vercel auto-deploy
- Test on live site
- Clear cache when needed: `Cmd+Shift+R` or `Ctrl+Shift+R`

### **Deploy Control:**
- Toggle `vercel.json` → `"deploymentEnabled": false` when making multiple changes
- Toggle back to `true` when ready to deploy

---

## 🎓 GLOSSARY

**Game Mode:** Progressive levels, must complete in order (1→2→3...)  
**Practice Mode:** Free selection, pick any level anytime  
**Module:** Complete game/learning experience (e.g., Algebra Expedition)  
**Level:** Single problem set within a module  
**Distractor:** Wrong answer choice designed to catch common mistakes  
**LevelIntro:** Story + teaching content before level starts  
**Progress Tracker:** UI showing which levels completed  
**Floating Icons:** Stats/info icons overlaid on game screen  

---

## 📞 CURRENT STATUS SUMMARY

**Where We Are:**
- ✅ Track 1 complete: Website live at ugmathtools.com
- 🔄 Track 2 ready to start: Copy Algebra Expedition
- 📋 22 issues identified and organized
- 🎯 Clear strategy: Surgical fixes, not rebuild
- ⏱️ Time budget: 8 hours maximum

**Next Immediate Step:**
Copy `/src/algebra` folder from old repo to new repo, verify it works

**Your Concerns Addressed:**
- ✓ Won't rebuild working code (levels 1-24 stay as-is)
- ✓ Won't risk regression (copy first, fix incrementally)  
- ✓ Won't exceed time budget (8 hours max, prioritized list)
- ✓ Will test continuously (after each fix)

**Michael's Mindset:**
- Don't want to rebuild ✓
- Don't want to debug for hours ✓
- Want to jump to the end ✓
- Already invested 100+ hours ✓
- Maximum 8 more hours ✓

**Claude's Role:**
- Provide step-by-step instructions
- Give complete file replacements (no diffs)
- Test after each change
- Keep it simple
- Stay within time budget

---

**END OF MASTER PLAN v1.3**

Last Updated: January 17, 2025 - 6:30 PM  
Next Review: After Track 2 Phase 1 complete  

---

## 📌 QUICK REFERENCE

**Your Repos:**
- Documentation: https://github.com/mrulmer-goodrich/UGMathTools-Documentation
- New Website: https://github.com/mrulmer-goodrich/UGMathTools-Website  
- Old MathTools: https://github.com/mrulmer-goodrich/MathTools

**Your Live Site:** https://ugmathtools.com ✓

**Your Vercel:** vercel.com/dashboard

**Current Focus:** Track 2 - Copy Algebra Expedition

**Next Step:** Copy `/src/algebra` folder to new repo

---

*This is your one living document. Everything important is here. When you're lost, come back to this. When we make decisions, this updates. You're crushing it, Michael. Track 1 done. Track 2 next.* 🚀
