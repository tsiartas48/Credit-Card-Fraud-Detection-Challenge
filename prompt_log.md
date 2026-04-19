# Prompt Log — Appendix B

## Session 1 — Βήμα 1: Problem Definition
**Εργαλείο:** Claude (Anthropic)
**Ημερομηνία:** 17/04/2026

**Prompt:** Σχεδιασμός αρχιτεκτονικής ML pipeline για fraud detection
**Output:** Ορισμός προβλήματος, επιλογή μετρικών (AUC-PR, F1), αναγνώριση class imbalance
**Κρατήθηκε:** Framework Βήματος 1, επιλογή μετρικών

---

## Session 2 — Βήμα 2: EDA
**Εργαλείο:** Claude (Anthropic)
**Ημερομηνία:** 17/04/2026

**Prompt:** Κώδικας για EDA στο Credit Card Fraud dataset
**Output:** Κώδικας για φόρτωση dataset, class distribution, amount analysis, correlation
**Κρατήθηκε:** Όλος ο κώδικας — 0 missing values, 0.173% fraud, V14 top feature

---

## Session 3 — Βήμα 3: Preprocessing
**Εργαλείο:** Claude (Anthropic)
**Ημερομηνία:** 17/04/2026

**Prompt:** Κώδικας για preprocessing, scaling, train/test split και SMOTE
**Output:** RobustScaler, stratified split 70/15/15, SMOTE για class imbalance
**Κρατήθηκε:** Όλος ο κώδικας

---

## Session 4 — Βήμα 4: Feature Engineering
**Εργαλείο:** Claude (Anthropic)
**Ημερομηνία:** 17/04/2026

**Prompt:** Feature selection με SelectKBest και Random Forest
**Output:** Top 20 features — V14 (22%), V4, V10, V17, V12
**Κρατήθηκε:** Top 20 features για model training

---

## Session 5 — Βήμα 5: Model Training
**Εργαλείο:** Claude (Anthropic)
**Ημερομηνία:** 17/04/2026

**Prompt:** Εκπαίδευση 4 αλγορίθμων — LR, RF, XGBoost, Neural Network
**Output:** Κώδικας εκπαίδευσης και αξιολόγησης
**Κρατήθηκε:** Όλος ο κώδικας — XGBoost καλύτερο (AUC-PR: 0.8149)

---

## Session 6 — Βήματα 6 & 7: Tuning & Ensemble
**Εργαλείο:** Claude (Anthropic)
**Ημερομηνία:** 17/04/2026

**Prompt:** RandomizedSearchCV για XGBoost και Voting Classifier
**Output:** Best params XGBoost, Ensemble με LR+RF+XGBoost
**Κρατήθηκε:** XGBoost Tuned (AUC-PR: 0.8245) — καλύτερο από Ensemble

---

## Session 7 — Βήματα 8, 9, 10: Evaluation
**Εργαλείο:** Claude (Anthropic)
**Ημερομηνία:** 19/04/2026

**Prompt:** Confusion matrix, ROC curve, learning curve, error analysis
**Output:** Test AUC-ROC: 0.9777, AUC-PR: 0.8187, F1: 0.7673
**Κρατήθηκε:** Όλος ο κώδικας και τα γραφήματα
