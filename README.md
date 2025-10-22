[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/oqKLEXJJ)
# 🎓 Ethical Admissions Algorithm Simulation

This repository is a classroom exercise exploring **ethics and fairness in algorithmic decision-making** — specifically in college admissions.

You’ll implement and reflect on how feature selection and weighting can impact fairness, transparency, and equity in automated systems.

---

## 🧩 Overview

You are part of the admissions committee for **Anonymous University**, located near Anonymous City.  
Due to a large number of applications, the committee decides to use an algorithm to help **rank and shortlist applicants**.

Your task:
- Decide which factors to include (GPA, test scores, extracurriculars, essays, recommendation letters, legacy status, income, etc.)
- Assign weights to each factor.
- Compare outcomes under two models:
  - **Blind model**: Ignores sensitive factors.
  - **Aware model**: Includes them intentionally to promote fairness (e.g., extra weight for first-gen or low-income applicants).

---

## ⚙️ How to Run

You can run the code on any online Java compiler (e.g. [Replit](https://replit.com/~) or [Programiz Java Compiler](https://www.programiz.com/java-programming/online-compiler))  
or locally via terminal:

```bash
javac Applicant.java Admissions.java Main.java
java Main


Answers to questions

Feature Selection and Design
I added a dependents variable because parents or guradians should still have a chance at attending even if their scores for tests or their GPA is a bit lower than the average.

I excluded legacy as a sensitive feature because it is not useful for judging the merit of the applicant.

No, legacy should not be carrying a positive weight, but should not be carrying a negative weight. The applicant should be judge on their merit rather than their relatives merit

I adjusted the GPA, to carry a bit more weight, and lowered the Extra Curriculars to carry half as much weight. Other factors that may need adjustment would be disability and local.

Fairness and Outcomes
Almost all applicants benefited. The only one that lost out was Hannah Miller.

Carlos Rivera, Fatima Al-Sayed, George Johnson, and Jasmine Okafor all benefited from the aware model.

Yes, I believe that adding income or first-generation make the system more fair. Income, helps elimate the stigma of wanting to keep the poor dumb, as well as the thought of having to buy your way into college, or that it should be a thing for the elite. First-generation, helps give students from families who are not educated, resources to help them better succeed in life and other areas that their relatives may not.

The aware model feels more fair because it brings in the "Human" aspect of the applicant and not just the "Analytical" aspect. It takes into account that their could have been other factors impacting the applicants GPA, test score, extra curriclars, etc.

Transparency and Accountability
I feel that the algorithm is pretty transparent. If someone were to read it, they shouldn't have a problem understanding what an applicant is addmitted on.

Yes, I could clearly explain why an applicant recieved a rejection for both the blind and aware models.

Yes, I would probably be comfortable if this algorithm evaluated my application because I feel, for the most part, that it fairly covers the areas in which an applicant's entry should be decided on.

Broader Implications
It would probably be biased in a way it wasn't intended to be

Credit and loan approval, healthcare, resource allocation, etc. 

It reveals that each algorithm has its own biases and what you define as fair is dependent on what your main objective is.

I think that there are too many factors in life and too many biases for an algorithm to be truly fair. The bias just shifts over time based on what humans determine to be fair.

Fairness and accountability should be designed to work together. Fairness ensures that algorithms prevent discrimination and allow room for explanation, while accountability focuses on responsibility for the outcomes. In either case, algorithms should remain transparent and subject to human oversight to ensure that decisions involve human judgment, not just mathematical processes.