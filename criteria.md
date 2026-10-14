# Acceptance criteria — TakeMeter

Five criteria that say what "working" means for this classifier, written in
unit 5 **before** anything was trained.

**All five are yours this time.** None are given. You've had two projects of
practice.

An acceptance criterion names a number. *"The model is accurate"* is an
opinion. *"Every label has an F1 of at least 0.60 on the held-out set"* is a
criterion.

Under each, write a sentence or two on **why that number**. A reason that says
something about your data or your taxonomy earns credit — *"I picked 0.60 F1
for `reaction` because it's my smallest label and I only have about 50
examples of it"*. A reason that could be attached to any project does not.

> Missing your own targets next unit costs you nothing. Setting a target so
> easy you can't miss it does.

---

## Pick numbers you can defend

Not numbers that sound impressive. Three labels means a coin-flip guesser gets
about 33%, so a target of 0.40 is barely a target. Your number should sit
somewhere you'd honestly call useful.

**Cover at least three of these five areas.** They're here as prompts, not as a
form to fill in — a criterion that fits none of them is fine if it names a
number.

| Area | A question it could answer |
|---|---|
| Overall accuracy | How often does it need to be right to be worth using? |
| Per-label performance | Is one label allowed to be much worse than the others? |
| Balance | How lopsided can your label counts get before it's a problem? |
| Consistency | If someone else labelled the same posts, how often should you agree? |
| Confidence | Should a confident prediction be right more often than an unsure one? |

Two things worth knowing before you pick numbers, because both will affect
whether you hit them:

- **Your smallest label will have the jumpiest score.** If a label has 50
  examples, about 8 land in the test split. An F1 computed on 8 examples moves
  a lot between seeds. A target for that label should be looser than one for
  your biggest label, and saying so is a good reason.
- **Unit 6 tests across three seeds, and the target has to hold across all
  three.** A target of 0.65 against results of 0.71, 0.62, 0.68 is a **miss**.
  Pick with that in mind — it is stricter than it first sounds.

---

## 1. Per-label performance

F1 score of at least 0.55 for each label is the goal.



**Why this target:**
Emotional Reaction label in a discussion forum page may lack a bit since people will mainly discuss their opinions on a song rather than just react with feelings, so at least 0.55 F1 score works.


---

## 2. Overall Accuracy

An overall accuracy of at least 70% is the goal. 



**Why this target:**

Being realistic about the number of examples (at least 200) and for a label like "Emotional Reaction" maybe lacking compared to the other two (could bring down accuracy), at least 70% accuracy will be good. 

---

## 3. Consistency

Agreement between annotators should be at least 90%. 



**Why this target:**

Don't want to much disagreement because that would mean the taxonomy defintions are not clear or decriptive enough. 90% is a good mark.

> **Revised in unit 6:** Beats the Baseline F1 per label 
>
> **Why revised:** This criterion was not a good fit for the project because the real decision question was whether the model outperformed the baseline on the label-level signals that mattered most. Since the taxonomy is uneven and the smallest label is unstable, evaluating improvement against the baseline F1 per label gives a more meaningful and measurable test than annotator agreement.

---

## 4. Balance

The largest label has to be less than or equal to 50%.

**Why this target:**
There are three labels, so if split evenly, it should be at least 33% each. However, if a label gets to more than 50%, it will dominate the other two (at most 25% each). 25% of 200 is 50, so anything less will leave so little for the test set. 


---

## 5. Confidence

Predictions at confidence ≥ 0.8 are correct ≥ 85% of the time



**Why this target:**
I chose this confidence target because predictions above the threshold should be reliable enough to use without checking every post. Lower-confidence predictions can be reviewed manually.

> **Revised in unit 6:** Dataset spread is less than 0.10
>
> **Why revised:** Confidence was not the main issue here because the model was not stable across seeds, and the spread in accuracy was the more important signal of whether the task was reliable. Since a spread above 0.10 means results shift too much depending on the random split, tracking dataset spread is a better measure of consistency for this project than checking confidence thresholds.
---

<!-- ─────────────────────────────────────────────────────────────────────────
     UNIT 6 — read this before you change anything above.

     If a criterion turns out to be BROKEN rather than merely unmet, you can
     revise it, and that earns credit. But never delete or edit the original
     line. Add the revision underneath, like this:

         ## 2. Every label performs acceptably

         The model performs well on all labels.

         **Why this target:** ...

         > **Revised in unit 6:** Every label has an F1 of at least 0.60 on
         > the held-out set.
         >
         > **Why revised:** "performs well" gave me nothing to check. I
         > couldn't produce a verdict from it at all.

     That's a revision because the criterion couldn't be MEASURED.

     Lowering a target because you missed it is not a revision, and it costs
     you the point:

         ✗ "Overall accuracy of at least 0.65" → "at least 0.55", because
            0.65 turned out to be optimistic for 200 examples.

     A number you missed stays where it is, gets diagnosed, and gets a fix
     attempted. That's where the points are.
     ───────────────────────────────────────────────────────────────────────── -->
