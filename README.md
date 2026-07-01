# 📚 ExamBuddy – Student Workflow

```text
Start
  │
  ▼
Login / Sign Up
  │
  ▼
Home Dashboard
(Welcome Card + Notifications)
  │
  ▼
Select Subject
  │
  ▼
Select Chapter
  │
  ▼
Choose Learning Mode
  │
  ├──────────────┬───────────────┐
  ▼              ▼               ▼
Revision   Concept Clarity   Knowledge Tester
```

---

# 📚 Revision

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

> **"Sun + Water + CO₂ = Plant Food + O₂"**

---

# 💡 Concept Clarity

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
> You can't order from Swiggy!

**Student:**

> I will cook by myself

**ExamBuddy:**

> Exactly! What **3 things** would you need from around you?


**Student:**

> Sunlight.

**ExamBuddy:**

> correct! You need energy to cook, and sunlight is free energy ☀️

**Progress:** `1 / 3 inputs identified`

> Now, plants are chefs. They mix ingredients. Sunlight is the stove.
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


### 🧠 Active Recall

**ExamBuddy:**

> Quick check — don't look at your textbook.
>
> Can you tell me the **three things** a plant needs for photosynthesis in your own words?

**Student:**

> Sunlight, carbon dioxide from the air, and water from the roots.


### ✅ Summary + Misconception Guard

**ExamBuddy:**

> Excellent! That's 100% correct.
>
> Plants use **sunlight, carbon dioxide, and water** to produce **glucose (food)** and release **oxygen**.
>
> This process is called **photosynthesis**.

**Common Exam Mistake**

> Many students write:
>
> *"Plants make oxygen for humans."*
>
> While that's true, it isn't the main purpose.
>
> In exams, write:
>
> **"The primary purpose of photosynthesis is to produce glucose (food) for the plant. Oxygen is a by-product."**

### 🎯 Exit Ticket

**ExamBuddy:**

> Final challenge...
>
> If I cover a plant's leaves with black paper for **3 days**, will photosynthesis happen?
>
> Why?

**Student:**

> No, because the leaves won't receive sunlight.

**ExamBuddy:**

> ✅ Mastered!
>
> I've updated your **Life Processes Mastery Map**.
>
> I'll remind you to revise this chapter again in **2 days** using spaced repetition so you remember it before your exams.

**Next Option**

> 📊 Show a 10-second concept diagram
>
> **OR**
>
> Continue to the next concept.

---

# 🧠 Knowledge Tester

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

---

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
