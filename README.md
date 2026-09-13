# SameExam

Live site: https://mjpalm13.github.io/same-exam/

Repo: https://github.com/Mjpalm13/same-exam

First AI commit, before I changed anything: https://github.com/Mjpalm13/same-exam/commit/d0ee442

This is a three-screen mock-up.

**Affordance sentence:** Find classmates already studying this exam tonight.

That line is the headline on the landing screen. The kicker above it is the value: Get unstuck tonight.

---

## Need, persona, capability, value

One sentence each. I kept them distinct: the need does not name the product, the capability is an action, and the value is the payoff after.

**Need**  
The night before an exam, students are already on campus and studying alone, they do not know who else from the class is nearby, and posting in GroupMe or walking the library usually burns the study block.

**Persona**  
Studies on campus 2-4 exam nights a semester, in 2-3 hour blocks between dinner and 10, carries a laptop, and wants one or two people from the same class rather than a big group.

**Capability**  
Find classmates who are studying this subject on campus tonight.

**Value**  
Learning. They get unstuck on the actual exam material instead of spinning alone.

---

## The three screens

I only built three, and I picked the ones that show the product working. No login, no settings, no "host a table" screen.

**Landing**  
Job: signal the capability and the value (learning / getting unstuck) at first glance.  
Why this screen: if this one is confusing, nobody even gets to the product.  
Design question: after five seconds, do they think this finds classmates on their exam tonight, or do they think it's a chat app they have to sign up for?

**Tonight's tables**  
Job: show the capability happening. Here's who is sitting down *now*, for *this* exam.  
Why this screen: this is the actual product. A profile page wouldn't tell me if the idea is clear.  
Design question: can they tell in a few seconds which table is worth walking to, based on what people are working on and where they are?

**Table**  
Job: show the value. This is your stuck point, so walk over and sit down.  
Why this screen: the list by itself is just browsing. This is the part where you decide you'd actually go.  
Design question: is "I'm walking over" obvious because the material and the people are grouped with that button, or does it still feel like you should message them first?

---

## Questions I would ask later

I'm not collecting answers yet. These are worded how I'd actually say them to someone in that persona. Next to each one is what I think they'll say, and which part of the prototype that guess is based on.

**Need.** "Okay so think about the last time you were on campus the night before a test, by yourself, and you kind of wanted someone from the class there. What did you end up doing?"

I think they'll say they posted in GroupMe or walked around the library looking for someone they recognized, then either studied alone or left. That's the situation the landing copy is about ("waiting on a class chat that never turns into a table") and it's why the STAT 230 card is on the first screen.

**Value.** "If that actually got solved for you on a night like that, what's one or two words for what you'd get out of it? Why those words?"

I think they'll say unstuck or learning, not "easier." That's why the table screen leads with what people are working on right now, not a map.

**Persona.** "How often does this even come up for you? And what are you usually doing when it does, like where are you and how much time do you have?"

I think it's only a few exam nights a semester, already on campus, dinner to 10, a couple hours to work. That's why the walk times are 3, 6, and 8 minutes, and why it says you don't need an account.

**Capability.** "I'm going to show you this first screen for five seconds and then hide it. What does this thing do?"

I think they'll say it shows who in their class is already studying tonight so they can go sit with them. That prediction is based on the big headline and the one button, "See who's studying tonight." If they say it's a social network or that you sign up to host tables, the landing is still competing with itself.

If I have time I'd also ask: "Click around for a second. What would you tap first, and what do you think happens?" I think they hit the orange button or the STAT 230 card and expect a list of tables they can walk to.

---

## First read (I opened my own live link like I hadn't seen it)

**Does the landing signal the capability and the value before you really read?**  
After I revised it, yes. You do not have to read the paragraph. The small line at the top says "Get unstuck tonight" (value: learning). The big headline is the affordance sentence / capability. One orange button. The card is classmates already on exam material, so the value is sitting there as an example, not as a second product.

**Does everything on the landing earn its place?**  
Now it does. "Get unstuck tonight" is the value before you read anything else. The paragraph under the headline is the GroupMe/walking-around problem. The card isn't decoration, it's proof that a table exists right now. "No account. If a table fits, you walk over." is there so people don't go looking for sign up. The first version did not pass this. I had two other buttons (host a table, create account) plus map/chat/calendar feature boxes, so nothing was the main job.

**What belongs together, and which Gestalt grouping did I use?**  
- Landing: figure-ground. Dark header and the orange button sit on the paper background so they come forward. The preview card is one common region. Inside it, proximity keeps "the exam" next to "the walk."  
- Tonight's tables: each table is its own common region (the card). Under the line, proximity puts people + what they're on in one cluster, and building + walk time in the other. Similarity: all three cards are laid out the same, so it still feels like one product.  
- Table screen: the learning panel is the focal point (thicker border, the main button lives in there). Place is a second region so you know where to go, but it shouldn't compete with getting unstuck.

**Do screens 2 and 3 stay on mission, and can you get back?**  
Yes. Tonight is only live tables. The table screen is only "is this my stuck point, and can I walk over?" Home and the SameExam name go back to the landing from everywhere.

**What the AI got wrong, and what I changed**  
The first pass looked like a mini social app. On the landing, "See who's studying tonight," "Host your own table," and "Create account" all had the same visual weight, so the primary capability didn't get signaled. Then there were three feature boxes for a map, chat, and calendar, which are secondary stuff I don't even have screens for. On the table screen the main button was "Message the table," which is literally the old workaround.

I changed it so there's one headline, one button, and the live table is proof, not another CTA. On the list, each card groups learning vs walk. On the table screen, "I'm walking over" sits in the learning cluster.

**Before and after**  
First landing: https://github.com/Mjpalm13/same-exam/blob/d0ee442/index.html  
Revised landing: https://github.com/Mjpalm13/same-exam/blob/main/index.html  

The problem wasn't "it looked generic." The hero gave equal weight to browse, host, and sign-up, so first glance didn't signal the primary capability. I cut the competing actions so finding a table is the thing you encounter. I grouped who + what they're on because if that information is scattered, people will read the list like a directory instead of a way to get unstuck.
