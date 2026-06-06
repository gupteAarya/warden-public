# Warden 

<img width="1024" height="500" alt="Stop Scrolling" src="https://github.com/user-attachments/assets/08e8404d-2790-4315-9e65-b03284712238" />

Warden is a simple yet powerful app designed to improve your morning routine. By reducing unnecessary phone usage during the most important hours of your day, it helps you stay focused, productive, and in control of your habits.

Warden is built to help you start your day with intention. Instead of getting trapped in endless scrolling, Warden encourages healthier habits and helps you focus on your morning goals.

## The Problem

Research suggests that smartphone and social media use around the sleep–wake cycle can negatively affect cognitive performance, sleep quality, mood, and daytime functioning. 
<br><br>
Experimental studies have found reduced working memory performance following social media scrolling, while sleep research links smartphone engagement near bedtime with delayed sleep and poorer next-day alertness.

Articles also indicate reduced attention span as another side effect.
<br>
[Electronic Media Use and Sleep Quality](https://pubmed.ncbi.nlm.nih.gov/38533835/), [Social media use, mental health and sleep](https://pubmed.ncbi.nlm.nih.gov/39242043/)

[Research by PubMed](https://pubmed.ncbi.nlm.nih.gov/36587230/) also shows increased sleep inertia due to imuplsive usage of social media in the morning, leading to a low productive day and reduced attention span. Chris Bailey's [Hyperfocus](https://chrisbailey.com/hyperfocus/) puts it best, "there's a finite limit on how many things we can focus on".

Together, these findings indicate that habitual morning bedscrolling interferes with the transition from sleep to focused, goal-directed activity, potentially disrupting productive morning routines.

## The SOLUTION

The solution is actually quite simple. The considerable significant effort required for productivity is actually just in order to overcome this inertia.
<br><br>
"If you do not open your sails, will you be able to harness the wind"
<br>
<img width="460" height="308" alt="graph" src="https://github.com/user-attachments/assets/ee7dba4e-04a4-485b-acf6-25f1ba361c2c" />
<br>
[Source](https://medium.com/illumination/motivation-unlocking-your-best-self-9b74caa7b3a2)
<br><br>
Quite poetically, your "Productivity Inertia" gained after overcoming sleep inertia helps you throughout your day.

Productivity inertia is the psychological and physical resistance to transitioning between states of work and rest. This inertia is what takes us through our work and is one of the responsible factors for us entering the flow state.

Warden is built around this very concept, to overcome sleep inertia and gaining productivity inertia.

## The IMPLEMENTATION

**Please note that this project is NOT VIBE-CODED**

Warden is designed to **reduce morning phone dependency** and help users **transition more effectively from sleep to productive activity**. By limiting access to distracting applications during the morning, Warden aims to **reduce** behaviors associated with **prolonged sleep inertia**, **attention fragmentation**, and **unintentional time loss caused by bedscrolling**.

To create a personalized focus period, Warden considers the following user-defined parameters:

* **Wake-up** time window
* Estimated **duration** of the **morning routine**
* **Additional focus time** desired after the morning routine

Based on these inputs, Warden **automatically restricts access** to **selected applications** for the calculated duration.

To ensure that essential functionality remains available, Warden includes an **Allowed Apps** list where users can add applications required for communication, navigation, productivity, or emergencies.

To encourage positive morning habits, Warden also provides an optional early-unlock mechanism. Users can scan items associated with their morning routine, such as:

* Toothbrush
* Coffee mug
* Study materials
* Laptop
* Books
* Other designated objects

Successfully completing these actions allows users to regain access to their device before the restriction period ends. This transforms routine morning activities into rewarding actions and creates a direct incentive to begin the day productively.

Together, these features help users establish momentum early in the day, reduce unnecessary screen time after waking, and build more intentional morning routines.

The application's features and implementation are described in detail in the following sections.

## Features

### WardenLock

<table>
<tr>
<td width="65%">

The apps core function. The **access restriction engine** that activates in the mornings to limit phone usage.

Its a completely **persistent, undismissable overlay** that stays on the screen until the scheduled time ends.

The overlay serves as the ***primary enforcement mechanism*** of Warden. During an active focus period, it is displayed as a **full-screen overlay** above restricted applications, preventing access until the restriction period expires or an approved **early-unlock action** is completed.

The overlay is designed to be **visually simple and distraction-free**. Rather than presenting excessive information, it focuses the user's attention on a small set of **essential elements**, including the remaining restriction time, the current focus objective, and available unlock options. This **minimalist design** discourages prolonged interaction with the device.

The overlay remains **persistent throughout** and automatically reappears whenever a restricted application is opened.

The overall design philosophy is centered around ***interruption rather than punishment***. Instead of overwhelming users with warnings or notifications, the overlay acts as a **gentle but unavoidable reminder** of the user's commitment to their morning routine and focus goals.

</td>
<td align="center">
<img src="https://github.com/user-attachments/assets/db6e9cbb-fe2f-4dc1-91be-54bf82eafb5b">
<br>
<em>The WardenLock Overlay</em>
</td>
</tr>
</table>

### Allowed Apps

<table>
<tr>
<td width="65%">

The apps core function. The **access restriction engine** that activates in the mornings to limit phone usage.

Its a completely **persistent, undismissable overlay** that stays on the screen until the scheduled time ends.

The overlay serves as the ***primary enforcement mechanism*** of Warden. During an active focus period, it is displayed as a **full-screen overlay** above restricted applications, preventing access until the restriction period expires or an approved **early-unlock action** is completed.

The overlay is designed to be **visually simple and distraction-free**. Rather than presenting excessive information, it focuses the user's attention on a small set of **essential elements**, including the remaining restriction time, the current focus objective, and available unlock options. This **minimalist design** discourages prolonged interaction with the device.

The overlay remains **persistent throughout** and automatically reappears whenever a restricted application is opened.

The overall design philosophy is centered around ***interruption rather than punishment***. Instead of overwhelming users with warnings or notifications, the overlay acts as a **gentle but unavoidable reminder** of the user's commitment to their morning routine and focus goals.

</td>
<td width="35%" align="center">
<img src="https://github.com/user-attachments/assets/db6e9cbb-fe2f-4dc1-91be-54bf82eafb5b" width="300">
<br>
<em>The WardenLock Overlay</em>
</td>
</tr>
</table>

- Scanner
- Morning Routine
- Statistics
- Habit Building
- etc.



## Screenshots

(images)

## Demo

(gifs)

## Architecture

(high-level diagram)

## Technical Stack

- Kotlin
- Compose
- Firebase
- etc.

## Testing

- Number of testers
- Bugs fixed
- Features added from feedback

## Privacy

High-level privacy principles.

## Roadmap

Future plans.

## Status

Actively maintained.
