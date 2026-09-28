# Study Buddy

Live site: https://mjpalm13.github.io/same-exam/

GitHub repo: https://github.com/Mjpalm13/same-exam

First AI commit, before I changed anything: https://github.com/Mjpalm13/same-exam/commit/d0ee442

## Product Description

Study Buddy is a three-screen mock-up for finding classmates who are already studying for the same exam nearby. Instead of creating a study group from scratch, you can see who is already studying, what they are working on, and where they are.


---

## 1. Need, Persona, Capability, and Value

**Need:**  
Many BYU students feel isolated and stressed right before exams because they do not know which classmates are studying at the same time. They usually study alone, message people they already know, or ask in a GroupMe, which takes time and does not guarantee that someone is actually available nearby.

**Persona (Last-Minute Leah):**

| **Name** | Leah Morgan |
| --- | --- |
| **Demographics** | **Age:** 21<br>**Gender:** Female<br>**Occupation:** College Student, majoring in Business |
| **Life Circumstances** | Leah is a junior who recently returned to BYU after serving a mission. She is living in an apartment near campus and is getting back into the routine of college life. Between classes, work, and other responsibilities, she does not always have a lot of time to study. She usually heads to the library with her laptop, notes, and class materials and tries to get as much done as possible before an exam. Since she has recently returned from her mission, she does not know many people in her classes very well yet. |
| **Personal Characteristics** | Leah usually studies alone, but she would rather have someone to work with when she gets stuck. She is comfortable reaching out to classmates, but she does not know many of them well enough to randomly message them about studying. She does not want to spend a lot of time trying to figure out who is available. When she gets stuck on a problem right before an exam, she wishes she could quickly see which classmates are studying for the same test and who is available and willing to work together. |
| **Goal** | Quickly find one or two classmates who are studying for the same exam right now so she can get unstuck, connect with classmates, and feel more prepared for the test. |

**Primary Capability:**  
Find classmates who are already studying for the same exam nearby.

The important part is that Leah can see who is already there instead of having to know people in her class or organize a study group from scratch. She can see who is studying, what they are working on, and where they are, then decide who she wants to join.


**Fundamental Value:**  
Connection! Leah can quickly go from studying alone to knowing that there are other students working through the same material nearby. This matters because she has recently returned to campus and does not know many people in her classes yet. Instead of spending her limited study time trying to find someone, she can connect with a classmate who is already studying and get unstuck.


---

## 2. The Three Screens


**Screen 1: Landing**
Page: index.html

Job: Explain what Study Buddy does and give the user one obvious thing to do.

Why it earned a slot: This is the first thing someone sees, so they should understand the idea quickly.

Design question: After looking at this screen for five seconds, would someone understand that Study Buddy helps them find classmates who are already studying tonight, or would they think it is just another social or chat app?

![Screen 1 landing](screenshots/screen-1-landing.png)

**Screen 2: Tonight’s Tables**
Page: tonight.html

Job: Show the main idea actually working. The user can see people who are already studying for the same exam and where they are.

Why it earned a slot: This is the part that makes Study Buddy different from just messaging people in a GroupMe. The student can see who is already studying instead of having to organize something themselves.

Design question: Can someone look at the different tables and quickly figure out which one they would actually want to walk to?

![Screen 2 tonight’s tables](screenshots/screen-2-tonight.png)

**Screen 3: Table Details**
Page: table.html?id=stat230

Job: Show what happens after someone finds a table. They can see who is there, what they are working on, and decide whether they want to join them.

Why it earned a slot: I wanted to show the actual moment where the student goes from "I am stuck" to "I found people who are working on the same thing."

Design question: Does seeing the people and what they are studying make going over to the table feel like the natural next step?

![Screen 3 table](screenshots/screen-3-table.png)

---

## 3. Design Question Plan

I am not collecting real answers yet. These are the questions I would ask someone who fits Leah's situation. I want to see if the problem is real to them and whether they understand the prototype without me explaining it.

### Need:

**Question:**
“Think about the last time you were on campus the night before a test, studying by yourself, and wished you had someone from your class there. What did you end up doing?”

**Prediction:**
I think they will say they messaged a GroupMe, texted someone they already knew, walked around the library hoping to recognize someone, or just kept studying alone.

**Based on:**
This prediction comes from the problem described on the landing page and the STAT 230 example showing students who are already studying.

### Value:

**Question:**
“If this problem were actually solved for you on a night like that, what would you get out of it?”

**Prediction:**
I think they will say connection, help, or getting unstuck. I do not expect them to describe the value as simply “easier” because the main benefit is being able to connect with someone who is already studying.

**Based on:**
The landing page leads with “Get unstuck with someone,” and the Table screen shows both the people and what they are working on.

### Persona:

**Question:**
“How often does this situation actually happen to you? Where are you usually studying when it does, and how much time do you normally have before the test?”

**Prediction:**
I think this comes up a few times during a semester, usually when they are already on campus with their laptop and have a couple of hours to study.

**Based on:**
Leah's situation and the nearby study locations shown on the Tonight's Tables screen.

### Capability:

**Question 1:**
“I am going to show you this first screen for five seconds, and then I will hide it. What would you say this thing does?”

**Prediction:**
I think they will say that it shows them who in their class is already studying tonight so they can go study with them.

**Based on:**
The headline, the “Get unstuck with someone” message, and the single main button, “See who's studying tonight.”


**Question 2:**
“Click around for a second. What would you tap first, and what do you think will happen?”

**Prediction:**
I think they will click the orange button or the STAT 230 example and expect to see classmates and study tables they can actually go to.

**Based on:**
The landing page gives the orange button the most attention, and the example table looks like the starting point for finding people.


---

## 4. Design Justification and First Read

After I made my changes, I opened the live site again and looked at it like I had never seen it before. I wanted to see if I could understand the main idea without thinking about what I had built behind the scenes.

### Does the landing screen signal the primary capability and value at first glance?

Mostly, yes. The first thing I notice is “Get unstuck with someone,” followed by “Find classmates already studying this exam tonight.” I think these work together because the first line gives me the value and the second tells me what I can actually do. The orange button is also the main affordance, so there is an obvious next step.

The example table also helps signal what the product does. Instead of just telling me that I can find classmates, I can immediately see an example of students already studying. I wanted the example to support the main idea without becoming another competing action.

### Does every element on the landing screen earn its place?

I think it does now. The first AI version had more features, including Browse, Host, Sign Up, chat, a map, and other options. These made the page feel more like a full social app and gave several actions similar visual weight.

I removed those because they were competing with the primary affordance. I wanted the landing screen to focus on one question: “Can I find a classmate who is already studying for the same exam?”

### What belongs together on each screen?

On the landing page, I used proximity to keep the main message and button together so they read as one main action. The example table is also grouped into a common region because it represents one opportunity to study with someone.

On the Tonight's Tables screen, each table is a separate common region. Inside each card, proximity groups the people with what they are studying. The building and walking time are also grouped together because they answer the question of where the table is and how easy it is to get there. Similarity between the cards helps them feel like different options within the same product.

On the Table screen, the people and study topic are grouped together because they help the student decide if this is the right group for them. The location is separated because it answers the next question: where do I go?

### Do screens 2 and 3 stay on mission?

Yes. The Tonight's Tables screen is focused on finding people who are already studying. The Table screen is focused on deciding whether that is a group the student wants to join.

I did not want either screen to turn into a full social or messaging app. The goal is to help the student find someone and actually go study with them.

I also made sure there is an obvious way back to the landing screen. The Study Buddy name and logo take the user back home from the other screens.

### What did the AI initially get wrong, and what did I change?

The first version the AI created was not bad visually, but it was trying to build too much. It treated Study Buddy more like a small social network instead of a focused way to find someone to study with.

The biggest problem was signaling. Browse, Host, and Sign Up all had similar visual weight, and there were also features for chat, a map, and other things. Because there were so many possible actions, the primary capability was not obvious.

I simplified the landing page to one main message, one main affordance, and one example of the capability working. This made the figure-ground relationship clearer because the important information stands out from the supporting content.

I also changed the main action on the Table screen from “Message the table” to “I’m walking over.” I made this change because messaging is already something students can do through GroupMe or text. The point of Study Buddy is to make it easier to find someone who is already studying nearby and actually go study with them.

### Before and after

The biggest change between the first AI version and my revised version was reducing the number of competing actions. I wanted the primary affordance to be visually dominant so a first-time user would understand what to do without needing an explanation.

**Before:** The landing page had Browse, Host, Sign Up, and extra features like chat and a map. These competed with the main idea.

[First AI landing screen](https://github.com/Mjpalm13/same-exam/blob/main/screenshots/landing-before.png) ([image](https://github.com/Mjpalm13/same-exam/raw/main/screenshots/landing-before.png))

**After:** I reduced the landing page to the main value, what Study Buddy does, one button, and an example table.

[Revised Study Buddy landing screen](https://github.com/Mjpalm13/same-exam/blob/main/screenshots/landing-after.png) ([image](https://github.com/Mjpalm13/same-exam/raw/main/screenshots/landing-after.png))

This revision was motivated by the design question of whether someone could understand the primary capability quickly. The first version had too many competing actions, while the revised version uses stronger signaling and grouping to make the main action easier to recognize.

First AI commit: https://github.com/Mjpalm13/same-exam/commit/d0ee442
Revised landing: https://github.com/Mjpalm13/same-exam/blob/main/index.html

