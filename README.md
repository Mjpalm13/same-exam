# SameExam

Three-screen mock-up for finding classmates who are already studying the same exam on campus tonight.

**Live prototype:** https://mjpalm13.github.io/same-exam/

**GitHub:** https://github.com/Mjpalm13/same-exam

**Initial AI commit (before revision):** https://github.com/Mjpalm13/same-exam/commit/d0ee442

**Affordance sentence:** Find classmates already studying this exam tonight.

---

## 1. Need, persona, capability, and value

**Need.** The night before an exam, students stall while studying alone and do not know who else in the class is already on campus and willing to work through the same material. They post in a class chat and wait, or walk the library hoping to spot someone, and lose the study block either way.

**Persona.** Prepares for exams in 2–3 hour campus blocks, two to four times a semester; wants one or two other people from the same class, not a huge group; usually between dinner and 10pm, laptop already in a library or building lobby.

**Capability.** Find classmates who are studying this subject on campus tonight.

**Fundamental value.** Learning. They get unstuck on the actual exam material with people in the same class, instead of spinning alone.

Need is the situation and the costly workaround. Capability is the observable action (find who is studying tonight). Value is the payoff after that action (learning / getting unstuck). The product is not named inside the need.

---

## 2. Three screens

| Screen | Job | Why it earned a slot | Design question it examines |
| --- | --- | --- | --- |
| **Landing** (`index.html`) | Signal the primary capability and the value *Learning* at first glance. | First-time users have to encounter the affordance sentence before anything else. If this screen fails, screens 2 and 3 never get a fair test. | After five seconds, do they know this helps them find classmates already on this exam tonight — or do they think it is a chat app / account product? |
| **Tonight’s tables** (`tonight.html`) | Demonstrate the capability: see who is sitting down *now*, for *this* exam. | This is the product working. A settings or host-a-table screen would not show whether the capability is clear. | Can they tell in a few seconds which table is worth walking to, using material + place rather than social noise? |
| **Table** (`table.html`) | Show the value in action: this is your stuck point, so walk over and sit down. | Completes the loop from “find” to “I would actually go.” Without it, the list is only browsing. | Does “I’m walking over” feel like the obvious next step because the learning cluster is grouped with the action? |

Three screens is a cap. Host, account, map, and chat did not earn a slot.

---

## 3. Design question plan

Questions I would actually say to this persona. Predictions only — not findings.

### Need

**What I would say:** “Think about the last night before an exam when you were on campus by yourself. What did you end up doing when you wanted someone from the class there?”

**Prediction:** They posted in GroupMe or walked HBLL looking for a familiar laptop sticker, then either studied alone or left. Rests on the landing copy (“waiting on a class chat that never turns into a table”) and the live STAT 230 preview.

### Value

**What I would say:** “If that problem were actually solved on a night like that, what’s one or two words for what you’d get out of it — and why those words?”

**Prediction:** “Unstuck” or “learning,” not “easier.” They care about the material on the table, which is why the table screen leads with *What they’re on right now* instead of a map.

### Persona

**What I would say:** “How often does this come up for you, and what are you usually doing when it does — like, where are you sitting and how much time do you have?”

**Prediction:** A few exam nights a semester, dinner to 10pm, already on campus with a laptop, 2–3 hour block. Rests on walk times (3 / 6 / 8 min) and “no account. If a table fits, you walk over.”

### Capability

**What I would say:** “I’m going to show you this first screen for five seconds, then hide it. What does this product do?”

**Prediction:** “It shows who in my class is already studying tonight so I can go sit with them.” Rests on the H1 affordance sentence and the single amber button *See who’s studying tonight*. If they say “it’s a study social network” or “you sign up to host tables,” the landing still has competing signals.

**Backup capability question:** “Click around. What would you tap first, and what do you expect would happen?”

**Prediction:** The amber button or the STAT 230 preview card; they expect a list of tonight’s tables, then a place they can walk to.

---

## 4. Design justification and first read

Opened the live URL as if I had never seen it.

**Does the landing signal capability and value before reading?** Yes, after the revision. The H1 is the affordance sentence. The only button is *See who’s studying tonight*. The preview card is a live example of classmates already on an exam, which is the value (learning at a real table) without introducing a second product.

**Does every landing element earn its place?** After the revision, yes. The kicker locates it in time (“Tonight on campus”). The lede names the costly workaround. The preview is not decoration; it is the capability in miniature. The line “No account. If a table fits, you walk over.” keeps secondary capability (hosting, accounts) off the screen so nothing competes with finding a table.

**What belongs together, and which Gestalt principle says so?**

- Landing: figure–ground — navy bar and amber button sit on paper; the preview is one *common region* for a single live table. Inside the preview, *proximity* splits “the exam” from “the walk.”
- Tonight’s tables: each card is a *common region*. A divider plus two clusters uses *proximity*: material + people stay together (the learning), place + walk time stay together (the logistics). *Similarity* of card structure makes the three tables one product.
- Table: the learning panel is the *focal point* (heavier border, primary action inside it). Place is a second region, close enough to support the walk, not competing with “get unstuck.”

**Do screens 2 and 3 stay on mission, and can you get home?** Yes. Tonight only lists live tables. Table only answers “is this my stuck point, and can I walk over?” Every screen has **Home** and the SameExam wordmark back to the landing.

**What the AI first pass got wrong, and what changed**

The first commit treated this like a small social product. On the landing, *See who’s studying tonight*, *Host your own table*, and *Create account* had equal visual weight, so nothing signaled the primary capability. A three-up feature row (map, chat, calendar) pulled attention to secondary tools. The table screen led with *Message the table*, which is the old GroupMe workaround, not the new capability.

Revision (this branch / PR): one affordance, one button, preview as evidence, cards grouped into learning vs walk, and *I’m walking over* placed inside the learning cluster.

**Before / after.** [Initial landing](https://github.com/Mjpalm13/same-exam/blob/d0ee442/index.html) vs [revised landing](https://github.com/Mjpalm13/same-exam/blob/main/index.html). The hero used to give equal weight to browse, host, and sign-up, so the first glance did not name the capability. The revised hero gives the affordance sentence and a single action; the live table is grouped as proof, not as a second CTA row.

The grouping change on tonight’s tables was motivated by the same design question: related things (who + what they’re on) must appear together, or people will scan this like a directory instead of a way to get unstuck.
