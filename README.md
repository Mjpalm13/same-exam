# Study Buddy

Live site: https://mjpalm13.github.io/same-exam/

GitHub repo: https://github.com/Mjpalm13/same-exam

First AI commit, before I changed anything: https://github.com/Mjpalm13/same-exam/commit/d0ee442

Study Buddy is a three-screen mock-up around a pretty simple idea: finding classmates who are already studying for the same exam nearby, so you are not stuck figuring out who to turn to.

**Affordance sentence:** Find classmates already studying this exam tonight.

That is the headline on the landing screen. The small line above it is the value: **Get unstuck with someone.**

---

## 1. Need, persona, capability, and value

I kept these four things separate. The need is the problem without naming the product. The capability is what you can actually do. The value is what is better afterward.

**Need**  
Nothing is worse than not knowing who to turn to for help, and if you don’t really know people in class, posting in a group chat or walking around looking for someone usually costs time and can feel embarrassing.

**Target persona**  
My target persona is already on campus the night before an exam and has a couple of hours to study. They usually end up studying alone, but they would rather work with one or two classmates when they get stuck. They have a laptop and class materials with them. They do not want to spend 30 minutes posting in a group chat, walking around looking for people, or trying to organize a study group. This is not someone looking for a new social network. They already have a reason to be on campus and a reason to study. Study Buddy is supposed to make it easier to connect with people who are already doing the same thing.

**Primary capability**  
Find classmates who are studying this subject on campus tonight.

The important part is that they can *see* who is already there instead of having to organize something from scratch.

**Fundamental value**  
Learning. The point is to get unstuck on the actual exam material instead of spinning alone.

How that value shows up in the experience:

- **Engagement:** they actually sit down with other people instead of studying completely alone.
- **Visibility:** they can see that other classmates are on the same material right now.
- **Usability:** finding someone is quick enough that it does not eat the study block they already have.

Learning is still the main value. Engagement, visibility, and usability are how the experience creates it.

---

## 2. The three screens

I only built three screens, and I chose the ones that show the idea actually working. I did not use a slot on login, settings, or “create a table,” because those would not tell me if the main idea is clear.

**Landing**  
Job: Signal the primary capability and the value as fast as possible.  
Why it earned a slot: If this screen is confusing, nobody gets to the product. The first thing they should get is that they can find classmates already studying this exam tonight, and that the payoff is getting unstuck with someone.  
Design question: After five seconds, do they understand that this finds classmates on their exam tonight, or do they think it is a chat app / social network they have to sign up for? Can they tell the opportunity to engage is visible enough to act on?

**Tonight’s tables**  
Job: Show the capability happening, and make other classmates visible. These are people studying right now for this exam.  
Why it earned a slot: This is the product working. A profile page would not tell me whether someone can actually see who is there and decide where to go.  
Design question: Can they quickly tell which table is worth walking to, based on what people are working on and where they are?

**Table**  
Job: Show the value in action. They see a stuck point, they see real people, and they can decide to go sit down.  
Why it earned a slot: The list by itself is mostly browsing. This is where they decide “this is what I need help with, and I can actually go there.”  
Design question: Does “I’m walking over” feel like the natural next step because the people and the material are grouped together, or does it still feel like they should message first?

---

## 3. Design question plan

I am not collecting answers yet. These are worded how I would actually say them to someone in that persona. Next to each one is what I think they will say, and which part of the prototype that guess comes from.

**Need**  
“Okay, think about the last time you were on campus the night before a test, by yourself, and you kind of wanted someone from class there but didn’t really know who to ask. What did you end up doing?”

I think they will say they posted in GroupMe, walked around the library looking for a face they recognized, or just stayed alone because asking felt awkward. That prediction comes from the landing paragraph (“not knowing who to turn to,” group chat / walking around, hassle and embarrassment) and from the STAT 230 card showing people who are already there.

**Value**  
“If that actually got solved for you on a night like that, what is one or two words for what you would get out of it? Why those words?”

I think they will say unstuck, learning, or something like “I’m not alone,” not “easier.” That is why the table screen leads with who is there and what they are working on, and why the kicker is “Get unstuck with someone.” If they say “I can see other people,” that is the visibility piece. If they say it has to be fast or they will not bother, that is usability.

**Persona**  
“How often does this even come up for you? And what are you usually doing when it does, like where are you and how much time do you have?”

I think this comes up a few exam nights a semester, when they are already on campus with a laptop and a couple of hours. That is why the walk times are 3, 6, and 8 minutes, and why there is no account.

**Capability**  
“I’m going to show you this first screen for five seconds and then hide it. What does this thing do?”

I think they will say it shows who in their class is already studying tonight so they can go sit with them. That prediction is based on the headline, the one button (“See who’s studying tonight”), the logo of two people studying together, and the live STAT 230 example. If they say it is a social network, a chat app, or something you sign up for, the landing is still competing with itself.

If I have time: “Click around for a second. What would you tap first, and what do you think happens?”  
I think they hit the orange button or the STAT 230 card and expect a list of tables they can actually walk to.

---

## 4. Design justification and first read

After I revised it, I opened the live site again like I had never seen it.

**Does the landing signal the capability and value at first glance, before reading?**  
I think it does now. You do not have to read the paragraph. The small line says “Get unstuck with someone” (learning + actually sitting with people). The big headline is the affordance sentence. One orange button. The card is classmates already on exam material, so visibility is an example, not a second product. The logo is two people grouped over one laptop, which is the same idea before you read any copy.

**Does every element on the landing earn its place?**  
After the revision, yes. The kicker is the value. The paragraph is the need: not knowing who to turn to, the hassle, the embarrassment. The card proves a table exists right now. “No account. Takes a minute. If it fits, you sit down.” is the usability piece, so people do not go looking for sign-up.

The first version did not pass this. I had “See who’s studying tonight,” “Host your own table,” and “Create account” all competing. I also had feature boxes for a map, chat, and calendar even though those were not part of the three screens. Looking back, I was trying to explain a whole app instead of communicating the one thing I wanted someone to understand.

**What belongs together, and which Gestalt grouping did I use?**  
- Landing: figure-ground. The dark header, logo, and orange button come forward on the paper background. The example table is one common region. Inside the card, proximity keeps who you’d sit with next to the walk. The logo and “Study Buddy” sit next to each other on purpose (proximity + similarity with the two-person idea).  
- Tonight’s tables: each table is its own common region. Inside the card, proximity groups people + what they are studying (should I engage?) and building + walk time (can I get there?). Similarity: all three cards use the same structure so they feel like one product.  
- Table: the “sit with them” panel is the focal point (thicker border, main button inside it). Place is a second region so you can answer a different question without it competing with getting unstuck.

**Do screens 2 and 3 stay on mission, and can you get home?**  
Yes. Tonight is only live tables you could actually join. The table screen is only “is this my stuck point, and can I walk over and sit down?” Home, the logo, and the Study Buddy name go back to the landing from everywhere.

**What the AI first got wrong, and what I changed**  
The first pass felt like a mini social app. The biggest problem was signaling, not that it “looked generic.” Browse, host, and sign-up had the same visual weight, so the primary capability was not obvious. Map / chat / calendar were extra. On the table screen the main button was “Message the table,” which is the old workaround.

I changed it to one headline, one button, and a live table as proof. I grouped people with the material they are on. “I’m walking over” sits in that cluster. Later I renamed it Study Buddy, put the two-person logo in the header, and rewrote the need so it is about not knowing who to turn to, not just “walking around wastes time.”

**Before and after**  
First AI version: https://github.com/Mjpalm13/same-exam/commit/d0ee442  
Initial landing: https://github.com/Mjpalm13/same-exam/blob/d0ee442/index.html  
Revised landing: https://github.com/Mjpalm13/same-exam/blob/main/index.html  

The first landing gave equal weight to browsing, hosting, and signing up, so nothing signaled the primary capability. I cut the competing actions. I also grouped who + what they’re on, because if that information is scattered, people will read the list like a directory instead of a way to get unstuck with someone.
