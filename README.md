# 📚 ExamBuddy – Student Workflow 

```text
Start
  │
  ▼
Login
  │
  ▼
Home Dashboard
  │
  ▼
Select Subject
  │
  ▼
Select Chapter
  │
  ▼
Select Topic
  │
  ▼
Concept ⇄ Notes (Content Screen - segmented control / swipe)
  │
  ├── 🤔 Ask Buddy (quick doubt, popup)
  │        └── "Teach me →" hands off to Concept Clarity
  │
  └── 📞 Call icon → Concept Clarity (guided, full screen)

Reachable from the bottom nav at any time:
Home · Concept/Notes (last mode) · Search · Knowledge Tester · Profile (incl. Test Results, Chats)
```

- **Concept ⇄ Notes** — a sticky segmented control at the top of the Content screen, swipeable, always on the same topic.
- **Knowledge Tester** — permanently one tap away via the bottom navigation bar, not tied to a specific topic selection.

### Offline vs Online — where the LLM actually runs

| Screen | Content source | Needs internet? |
|---|---|---|
| **Concept tab** | Pre-built, offline — bundled with the app per student's class/curriculum | ❌ No |
| **Notes tab** | Pre-built, offline — bundled with the app per student's class/curriculum | ❌ No |
| **Ask Buddy** | RAG + LLM, generated live | ✅ Yes |
| **Knowledge Tester** (MCQ + Short Answer) | RAG + LLM, generated/evaluated live | ✅ Yes |
| **Concept Clarity** ("Teach me" mode) | RAG + LLM, generated live | ✅ Yes |

Concept and Notes are authored once per class/curriculum and shipped with the app, so a student can open and read them without a connection. The LLM only comes into play the moment a student wants something dynamic — asking a doubt, taking a test, or going into a guided Socratic lesson.

---

# 📖 Content Screen: Concept ⇄ Notes (Offline)

```text
Select Topic
      │
      ▼
Content Screen opens
      │
      ▼
Load pre-built notes for this
topic (bundled per class, offline)
      │
      ├── Concept tab (paged, per sub-topic)
      │     • Clean headings
      │     • Visual thinking prompts
      │     • Simplified explanations
      │     • Prev / Next pager, page count (e.g. 9/19)
      │
      └── Notes tab (continuous chapter scroll)
            • Quick recap per topic
            • Key points, formulas, mnemonics
            • Auto-scrolls to the topic just opened
      │
      ▼
Switch anytime via the segmented control or a swipe —
same topic, no re-navigation
```

**Header:** shows the chapter number + name (e.g. "7. Magnetism") — this is sticky and shared by both tabs, so neither tab repeats it in its own content.

**Topic list:** every chapter now also lists an **"X.0 — Introduction"** row above its numbered topics. Tapping a topic (e.g. 7.1) lands directly on that topic's content; tapping the Introduction row lands on the chapter's intro section specifically.

### Example — Selected topic: Water Pollution (Concept tab)

> **🌊 Stop for a second...**
>
> Imagine a clean lake. Fish are swimming. Birds are drinking water.
> Now imagine people throwing plastic, sewage and chemicals into the same lake.
> Would you still drink that water? Probably not.
> That is exactly what **Water Pollution** means.

**Definition** — Water pollution is the contamination of water bodies due to human activities. It occurs when harmful substances like chemicals, sewage and waste are released into water bodies, making the water toxic and unsafe to drink.

**Sources** — Household detergents · Domestic sewage · Agriculture · Industrial waste · Oil spills · Thermal pollution

**Exam Keywords** — Pollutants · Aquifers · Domestic Sewage · Eutrophication · Oil Spill · Thermal Pollution

### Same topic, Notes tab (quick recap)

✅ **Quick Recap**
- Water pollution = contamination of water bodies by human activity.
- Main sources: sewage, industrial waste, agriculture, oil spills.
- Leads to toxic water and health risks.

✅ **Memory Trick**
> **"Sewage + Chemicals + Waste = Polluted Water"**

---

# 🤔 Ask Buddy — Quick Doubt Solver (Popup, Online)

Ask Buddy is reached from the **"🤔 Ask"** button in the Content screen header. It behaves like a search-engine or ChatGPT-style quick lookup, not a lesson — short, direct answers, with follow-ups offered rather than forced.

```text
Tap "Ask"
      │
      ▼
Popup opens over the Content screen
      │
      ▼
Student types or taps the voice button
      │
      ▼
Retrieve relevant content (RAG)
      │
      ▼
LLM gives a short, direct answer
• What it is / why it happens / how it works
• No guiding questions, no forced lesson flow
• Optional follow-up suggestion offered, not required
      │
      ▼
Student returns to studying
      │
      ▼
(Optional) "💬 Teach me →" hands off to Concept Clarity
             for a full guided lesson on the same doubt
```

### Composer (shared design with Concept Clarity)

- **"+"** on the left — reserved for future attachments.
- Placeholder: *"Ask your doubts…"*
- Right-side button morphs between a **waveform (voice)** icon and a **send** icon the instant the student starts typing, and reverts to voice once the message is sent.

### Example

**Student asks:**
> What is photosynthesis?

**Ask Buddy:**
> **Photosynthesis** is the process plants use to make their own food, using sunlight, carbon dioxide and water.
>
> Want the exam-definition wording, or a quick real-life example? Just ask 👇

That's the whole exchange — no Socratic build-up, no multi-turn questioning. If the student wants the deeper walkthrough, they tap **"Teach me →"** and land in Concept Clarity.

---

# 💬 Concept Clarity — Guided Teaching Mode (Full Screen, Online)

Reached via the **📞 call icon** on the Content screen header, or via **"Teach me →"** from Ask Buddy. This is the one-to-one Socratic lesson experience — same composer component as Ask Buddy (identical layout, icons, placeholder swapped to *"Let's understand better…"*), but a completely different response style and pacing.

```text
Open Concept Clarity
      │
      ▼
Retrieve textbook content (RAG)
      │
      ▼
LLM starts a Socratic conversation
• Real-life analogy first
• One idea at a time, short conversational messages
• Guiding questions instead of direct answers
• Progress bar fills in live as understanding is checked
      │
      ▼
Concept Check → Summary card + Misconception guard
      │
      ▼
Mastery Toast — Mastery Map updated
      │
      ▼
Lesson continues naturally through chat —
no separate "Continue" or "Show diagram" buttons
```

### Example

**Student asks:**
> What is Photosynthesis?

**ExamBuddy:**
> Excellent topic! This concept is frequently asked in exams, so understanding it well will help you score better.
>
> Before we break it down, imagine you're a plant stuck in one spot all day. How would *you* get your own food?
>
> You can't order from Swiggy 😀

**Student:** I will cook by myself

**ExamBuddy:** Exactly! Just like that, plants also cook their own food. This process is called **photosynthesis**.
> Now — what do you think a plant needs to "cook" with? Take a guess.

**Student:** Sunlight.

**ExamBuddy:** Nice thinking — sunlight is one of them ☀️ You need energy to cook, and sunlight is free energy.
`1 / 3 inputs identified`
> There's also a gas from the air involved. Any guesses on the gas?

**Student:** Carbon dioxide!

**ExamBuddy:** That's it — **carbon dioxide**! 🎉
`2 / 3 inputs identified`
> Plants don't have taps though — where do you think they secretly pull water from?

**Student:** Through the roots.

**ExamBuddy:** Nailed it — **roots** are basically the plant's straws! 🌱
`3 / 3 inputs identified`
> Sunlight + CO₂ + water → photosynthesis. Say it back to me in your own words — you've basically got it already.

The conversation continues turn by turn — entirely through the chat composer (text or the voice shortcut), with no navigation buttons required to move the lesson forward.

---

# 🧠 Knowledge Tester (Online)

Reached anytime via the **Test** icon in the bottom navigation — no longer tied to selecting a topic first.

## MCQ

```text
Tap "Test" in bottom nav
      │
      ▼
Start Quiz
      │
      ▼
Answer MCQs
      │
      ▼
Instant Score + Explanation
      │
      ▼
Next Question
```

**Question:** Which gas is absorbed by plants during photosynthesis?
A. Oxygen  B. Nitrogen  C. Carbon Dioxide  D. Hydrogen

**Student Answer:** ✅ Carbon Dioxide
**ExamBuddy:** ✔ Correct! Plants absorb carbon dioxide from the atmosphere through stomata to prepare glucose during photosynthesis.

## Short Answer

```text
Record Answer
      │
      ▼
Speech → Text
      │
      ▼
Retrieve Reference Answer (RAG)
      │
      ▼
LLM Compares Answers
      │
      ▼
Score + Feedback
      │
      ▼
Identify Missing Concepts
```

**Question:** Explain the role of stomata in the process of photosynthesis.
**Student (voice):** Stomata are tiny pores on the leaves which take in carbon dioxide from the air and release oxygen.
**ExamBuddy:** ✅ Good attempt! 1.5 / 2 Marks
- ✔ Correctly mentioned gas exchange
- ✔ Explained carbon dioxide intake
- ✔ Mentioned oxygen release
- ❌ To score full marks, also mention that **stomata regulate water loss through transpiration**.

**Test Results** (past scores, accuracy, marks) are archived under **Profile → Test Results** for review anytime, separate from taking a new test.

---

# 👤 Profile & Supporting Screens

```text
Bottom Nav
  │
  ├── Home — streaks, mastery ring, subjects
  ├── Concept/Notes — reopens whichever tab the student was last on
  ├── Search — live filter across chapters and topics
  ├── Test — jumps straight into Knowledge Tester
  └── Profile
        ├── Stats — day streak, overall mastery, topics done
        ├── Test Results — past scores, accuracy, marks
        ├── Your Chats — past conversations, grouped by subject
        └── Settings — notifications, language, help, log out
```

---

# Overall AI Workflow

```text
Student
   │
   ▼
Subject → Chapter → Topic
   │
   ▼
Content Screen
   │
   ├── Concept tab ──────┐
   │                     ├── Offline — pre-built notes, bundled per class
   └── Notes tab ─────────┘        (no internet required)

   ├── Ask Buddy (popup) ──────────── Online — RAG → LLM → Short, direct answer
   │
   ├── Concept Clarity (full screen) ── Online — RAG → LLM → Socratic conversation
   │
   └── Knowledge Tester (bottom nav, any time) ── Online
          ├── MCQ Engine → Instant Feedback
          └── Voice Answer → Speech-to-Text → RAG → LLM → Evaluation & Feedback
```

---

# Prototype

- [link](https://raguram-n.github.io/Exam_Buddy_Student_Screen/)
