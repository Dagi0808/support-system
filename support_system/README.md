# Human-in-the-Loop AI Customer Support System

A real-world NLP project built from scratch using RNN → Attention → Transformer.

## Problem
Customers send messages about delivery, finance, education, and account issues.
The system understands the message, checks the database, and either responds
automatically or routes it to a human worker for confirmation.

## Tech Stack
| Component      | Technology              |
|----------------|-------------------------|
| Programming    | Python                  |
| Deep Learning  | PyTorch                 |
| Data           | Pandas, NumPy           |
| API            | FastAPI                 |
| Interface      | HTML, CSS, JavaScript   |
| Version Control| Git, GitHub             |
| Evaluation     | Accuracy, Precision, Recall, F1 |

## Categories
- DELIVERY — 7 sub-intents — 100 messages
- FINANCE   — 5 sub-intents — 80 messages
- EDUCATION — 5 sub-intents — 70 messages
- ACCOUNT   — 5 sub-intents — 50 messages

## Build Stages
- [ ] Step 1  — Dataset (300 labeled messages)
- [ ] Step 2  — SQLite Database + sample data
- [ ] Step 3  — Tokenizer
- [ ] Step 4  — RNN Classifier
- [ ] Step 5  — Attention Layer
- [ ] Step 6  — Transformer Block
- [ ] Step 7  — Connect models to database
- [ ] Step 8  — Business logic + routing rules
- [ ] Step 9  — FastAPI backend
- [ ] Step 10 — Worker dashboard
- [ ] Step 11 — Customer chat interface
- [ ] Step 12 — Evaluate all 3 models

## Project Structure
```
support_system/
├── data/
│   ├── messages.csv         ← 300 labeled messages
│   └── database.db          ← SQLite
├── models/
│   ├── rnn_classifier.py
│   ├── rnn_attention.py
│   └── transformer.py
├── engine/
│   ├── tokenizer.py
│   ├── trainer.py
│   └── predictor.py
├── app/
│   ├── main.py
│   ├── routes/
│   │   ├── customer.py
│   │   └── worker.py
│   └── business_logic.py
├── dashboard/
│   ├── index.html           ← worker dashboard
│   └── chat.html            ← customer chat
└── evaluate/
    └── compare_models.py
```
