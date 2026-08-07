# CS2005 — Database Systems
Starts easy, cramming-heavy at first, then gets legitimately hard once normalization and concurrency show up. Lab (CL2005) does more heavy lifting for SQL than the theory course does.

## Overview
Pace is fine but front-loaded with memorization — intro chapters (DB approach, data models, 3-schema architecture) are basically diagram-cramming. Things click once you're doing SQL and ER modeling. By Mid1 you've covered basic SQL; by Mid2, joins/aggregates, ER modeling, relational algebra, and normalization. Final term brings transaction processing and concurrency control, which overlaps heavily with your OS course (locking, etc.) — useful synergy if you're taking both.

One quirk: CL2005 (the DB lab) goes deeper into SQL than CS2005 theory lectures do, but the exam still expects lab-level SQL knowledge. So don't treat theory and lab as separate prep tracks, the lab tasks basically *are* your SQL prep.

## Topics & Resources

### Intro & Data Models (Ch1, Ch2)
- Key idea: DB approach vs files, 3-schema architecture, data independence, DBMS classification.
- Honestly just cramming/memorization territory — a lot of diagrams to memorize rather than concepts to understand.

### Relational Model & Constraints (Ch5)
- Key idea: relational model concepts, constraints, referential integrity, transactions, constraint violations.
- Referential integrity etc. was hard to grasp initially — a few YouTube videos (no specific one saved, sorry) made it click. If you're stuck here, just go find explainer videos rather than re-reading the textbook.

### SQL — DDL, Retrieval, DML, Views (Ch6, Ch7)
- Key idea: SQL data definition/constraints, basic + complex retrieval queries, INSERT/DELETE/UPDATE, views, schema changes.
- Doing the CL2005 lab tasks yourself covers this — no separate theory prep needed if you actually do the lab work instead of copying it.
- Extra practice: [CS50SQL](https://cs50.harvard.edu/sql/) — Week 0 (Querying) and Week 1 (Relating) map almost exactly onto Ch5/6/7.

### ER Modeling (Ch3)
- Key idea: entity types, relationships, structural constraints, ER diagrams, naming conventions, higher-degree relationships.
- Easy once the concept clicks: read the scenario, underline the verbs — those are your relationships. Use **Chen's notation** for ERDs, not crow's foot (exam expects Chen's).
- Watch: [playlist](https://www.youtube.com/playlist?list=PLq-1NzkC-4DwTSmQa0dAN0r_3wWhg8kv9), then [this recap video](https://youtu.be/LowjDtiNlk4?si=dQos1QuClvav1oKD) for a shorter version.

### Relational Algebra (Ch8)
- Key idea: SELECT, PROJECT, JOIN, DIVISION and other set-theory-based operations.
- Best learned off the slides + lots of practice problems. The DIVISION operator specifically is the hard part — budget extra time for it.
- Watch: [video 1](https://youtu.be/yWxCz8wi0fM?si=bhMg4lLdXxNjyrXv), [video 2](https://youtu.be/CSI5NStnhDs?si=-UFo6-dcdECMSCvb)

### Normalization (Ch14)
- Key idea: functional dependencies, 2NF/3NF/BCNF, multivalued dependencies, 4NF/5NF.
- The hardest topic. Practice a LOT of questions, especially 0NF→1NF and 2NF — that's where exam questions actually bite. 4NF/5NF was barely tested in this offering — confirm with your own teacher before sinking time into it.
- Watch: [playlist](https://www.youtube.com/playlist?list=PLyp-1WQY32mN6U6PUq9c977X9vyHxtohD), then [video 1](https://youtu.be/GFQaEYEc8_8?si=Ij59aiCOtqroC9V6) and [video 2](https://youtu.be/VWnKUKH4tLg?si=iUhIdy1-8dWIsz_z)

### Transaction Processing, Concurrency Control & Recovery (Ch20, Ch21, Ch22)
- Key idea: ACID properties, schedules/serializability, 2PL and other concurrency control techniques, locking granularity, recovery methods (NO-UNDO/REDO, deferred/immediate update).
- Overlaps with OS course content (locking etc.) — if you've done that unit in OS already, it'll feel familiar.
- Watch: [Gate Smasher's playlist](https://youtube.com/playlist?list=PLxCzCOWd7aiFAN6I8CuViBuCdJgiOkT2Y&si=wvW0gXEMXHvUIkh6), starting from lecture 87 onward — but cross-check against your own course slides so you don't study beyond the syllabus.

### NoSQL (Ch24)
- Key idea: (left for someone else to fill in, wasn't covered in this offering of the course)

## Tips

**Biggest mistake:** leaving SQL prep for the end. Your concepts won't have time to actually form, and you'll struggle in the exam. Solve the CL2005 lab tasks yourself as you go instead of just copying — that's your real SQL prep.

**Exam structure** (sessionals and final, roughly consistent):
- Q1: theory concepts, usually multi-part
- Q2: SQL queries — a table/schema is given, then queries based on it
- If normalization is on the exam: one big question on it, 0NF through 3NF
- If ERD is on the exam: one big question — draw an ERD from a scenario
- If relational algebra is on the exam: same format as Q2 (table given, then queries), sometimes combined with SQL
- Later-chapter topics (transactions/concurrency/recovery): graphs, lock-checking exercises, etc. — basically anything fair game from the syllabus, but this is the general shape

**If you're short on time:** don't get stuck on a SQL query you can't immediately think of. Do what you know first, then come back to it — SQL queries eat time if you sit and stare, and you'll fall behind on the rest of the paper.

## Useful Links
- Trek's own **past papers** and **notes** sections for this course — read the notes, solve the past papers. This was called out as the single most useful external resource.
- [CS50SQL](https://cs50.harvard.edu/sql/) (Week 0 & Week 1) for extra SQL practice alongside Ch5/6/7
- ER Modeling: [playlist](https://www.youtube.com/playlist?list=PLq-1NzkC-4DwTSmQa0dAN0r_3wWhg8kv9) + [recap video](https://youtu.be/LowjDtiNlk4?si=dQos1QuClvav1oKD)
- Normalization: [playlist](https://www.youtube.com/playlist?list=PLyp-1WQY32mN6U6PUq9c977X9vyHxtohD) + [video 1](https://youtu.be/GFQaEYEc8_8?si=Ij59aiCOtqroC9V6) + [video 2](https://youtu.be/VWnKUKH4tLg?si=iUhIdy1-8dWIsz_z)
- Relational Algebra Division Operator: [video 1](https://youtu.be/yWxCz8wi0fM?si=bhMg4lLdXxNjyrXv) + [video 2](https://youtu.be/CSI5NStnhDs?si=-UFo6-dcdECMSCvb)
- Transactions/Concurrency/Recovery: [Gate Smasher playlist, lecture 87+](https://youtube.com/playlist?list=PLxCzCOWd7aiFAN6I8CuViBuCdJgiOkT2Y&si=wvW0gXEMXHvUIkh6)
