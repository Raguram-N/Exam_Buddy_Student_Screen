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
Select topic
  │
  ▼
Select Mode
  │
  ├──────────────┬──────────────────┬───────────────┬
  ▼              ▼                  ▼               ▼
Revision Mode    Concept Notes    Concept Clarity   Knowledge Tester
(Offline)        (Offline)          (Online)            (Online)
```

---

# 📚 Mode 1: Revision  - Quick recap

```text
Select Chapter
      │
      ▼
Retrieve Content (RAG)
      │
      ▼
LLM Generates
• Quick Recap
• Key Points
• Formula Cards
• Mnemonics
      │
      ▼
Revision Complete
```

### Example

**Selected Chapter:** Photosynthesis

**ExamBuddy generates:**

✅ **Quick Recap**

- Photosynthesis is the process by which green plants prepare food.
- Chlorophyll traps sunlight.
- Carbon dioxide enters through stomata.
- Water is absorbed by roots.
- Glucose is produced and oxygen is released.

✅ **Quick Formula**

```
Carbon Dioxide + Water + Sunlight
            ↓
 Glucose + Oxygen
```

✅ **Memory Trick**

> **"Sun + Water + CO₂ = Glucose (Plant Food) + O₂"**

---

# 📖 Mode 2 — Concept Notes

```text
Select Chapter
      │
      ▼
Select topic
      │
      ▼
Retrieve textbook content (RAG)
      │
      ▼
LLM transforms textbook into
student-friendly notes
      │
      ▼
Generate

• Clean headings
• Better formatting
• Visual thinking prompts
• Simplified explanations
• Important keywords
• One-minute chapter summary
      │
      ▼
Study Complete
```

## Example Selected topic: Water Pollution

### Our concept notes

> **🌊 Stop for a second...**

Imagine a clean lake.

Fish are swimming.

Birds are drinking water.

Now imagine people throwing plastic, sewage and chemicals into the same lake.

Would you still drink that water?

Probably not.

That is exactly what **Water Pollution** means.

---

### Definition

Water pollution is the contamination of water bodies due to human activities.

It occurs when harmful substances like chemicals, sewage and waste are released into water bodies.

Result

- Water quality changes
- Water becomes toxic
- Drinking polluted water affects human health

---

### Sources

Household detergents

Domestic sewage

Agriculture

Industrial waste

Oil spills

Thermal pollution

---

### Exam Keywords

- Pollutants
- Aquifers
- Domestic Sewage
- Eutrophication
- Oil Spill
- Thermal Pollution

---

# 💡 Concept Clarity mode - Dive deep

```text
Select Chapter
      │
      ▼
Ask Question
(Text /Voice)
      │
      ▼
Retrieve Textbook Content (RAG)
      │
      ▼
LLM Generates
Socratic Conversation
      │
      ▼
Concept Check
      │
      ▼
Summary + Misconception Guard
      │
      ▼
Exit Ticket
      │
      ▼
Update Mastery Progress
```

## Example

**Student asks:**

> What is Photosynthesis?

**ExamBuddy:**

> Good question — this one shows up in every exam.
>
> Before we break it down: imagine you're a plant stuck in one place all day. How would you get your own food?
>
> You can't order from Swiggy 😀!

**Student:**

> I will cook by myself

**ExamBuddy:**

> Exactly! Just like you, plants also cook their own food. That cooking process is called **photosynthesis**.

> What three things would a plant need to cook its food?


**Student:**

> I think, one is Sunlight.

**ExamBuddy:**

> correct! Plants need energy to cook, and sunlight is free energy ☀️

**Progress:** `1 / 3 inputs identified`

> Now, Imagine plant as chefs. They mix ingredients. Sunlight is the stove.
>
> What gas from the air do you think is their main ingredient?
>
> **Hint:** We breathe it out when we exercise.


**Student:**

> Carbon dioxide.

**ExamBuddy:**

> Perfect! CO₂ in, O₂ out — that's why plants are called Earth's lungs.

**Progress:** `2 / 3 inputs identified`

> Last one: The stove and gas aren't enough. A chef needs water too.
>
> Plants don't have taps.
>
> Where do they secretly pull water from?


**Student:**

> Through their roots.

**ExamBuddy:**

> Nailed it! 🌱
>
> Roots are like the plant's straws.


The conversation continues naturally until the student fully understands the concept.

---

# 🧠 Knowledge Tester mode 

## MCQ

```text
Start Quiz
      │
      ▼
Answer MCQs
      │
      ▼
Instant Score
      │
      ▼
Explanation
      │
      ▼
Next Question
```

### Example

**Question**

Which gas is absorbed by plants during photosynthesis?

A. Oxygen

B. Nitrogen

C. Carbon Dioxide

D. Hydrogen

**Student Answer**

✅ Carbon Dioxide

**ExamBuddy**

✔ Correct!

**Explanation**

Plants absorb carbon dioxide from the atmosphere through stomata to prepare glucose during photosynthesis.


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

### Example

**Question Display**

> Explain the role of stomata in the process of photosynthesis.

**Student Voice Answer**

> Stomata are tiny pores on the leaves which take in carbon dioxide from the air and release oxygen.

**ExamBuddy**

✅ **Good attempt! 1.5 / 2 Marks**

### Feedback

✔ Correctly mentioned gas exchange.

✔ Explained carbon dioxide intake.

✔ Mentioned oxygen release.

❌ To score full marks, also mention that **stomata regulate water loss through transpiration**, which is an important function described in the textbook.

---

# Overall AI Workflow

```text
Student
   │
   ▼
Subject Selection
   │
   ▼
Chapter Selection
   │
   ▼
Learning Mode
   │
   ├── Revision
   │      │
   │      └── RAG → LLM → Quick Recap Cards
   │
   ├── Concept Clarity
   │      │
   │      └── RAG → LLM → Socratic Conversation
   │
   └── Knowledge Tester
          │
          ├── MCQ Engine → Instant Feedback
          │
          └── Voice Answer → Speech-to-Text → RAG → LLM → Evaluation & Feedback
```

---

# Prototype 

- [link](https://raguram-n.github.io/Exam_Buddy_Student_Screen/)
