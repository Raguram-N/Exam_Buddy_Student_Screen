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

## 📚 Revision

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

---

## 💡 Concept Clarity

```text

Select Chapter
      │
      ▼
Ask Question
(Text / Voice)
      │
      ▼
Speech → Text 
      │
      ▼
Retrieve Textbook Content (RAG)
      │
      ▼
LLM Explains
      │
      ▼
Socratic Conversation
      │
      ▼
Concept Understood
```

---

## 🧠 Knowledge Tester

### MCQ

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

### Short Answer

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
## Example: 
- **Question display:** Explain the role of stomata in the process of photosynthesis.
- **Student voice answer:** Stomata are tiny pores on the leaves which take in carbon dioxide from the air and release oxygen.

**Our agent: Good attempt! 1.5 / 2 Marks**

> You correctly mentioned gas exchange. To get full marks, also mention that stomata regulate water loss (transpiration).

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
   ├── Revision → RAG → LLM → Quick Recap
   │
   ├── Concept Clarity → RAG → LLM → Conversational model
   │
   └── Knowledge Tester
           ├── MCQ Engine
           └── Voice Answer → RAG → LLM → Evaluation
```
