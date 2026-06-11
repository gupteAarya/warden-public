# Warden 

<img width="1024" height="500" alt="Stop Scrolling" src="https://github.com/user-attachments/assets/08e8404d-2790-4315-9e65-b03284712238" />

Warden is a simple yet powerful app designed to improve your morning routine. By reducing unnecessary phone usage during the most important hours of your day, it helps you stay focused, productive, and in control of your habits.

Warden is built to help you start your day with intention. Instead of getting trapped in endless scrolling, Warden encourages healthier habits and helps you focus on your morning goals.

[Visit the Website](https://wardenlanding.vercel.app/)
. The App will soon be available for download on the Google Play Store.

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
<td width="35%" align="center">
<img alt="WardenLock Overlay" src="https://github.com/user-attachments/assets/db6e9cbb-fe2f-4dc1-91be-54bf82eafb5b">
<br>
<em>The WardenLock Overlay</em>
</td>
</tr>
</table>

### Morning Routine Scanner

<table>
<tr>
<td width="65%">

The only way to complete a **WardenLock session** early is by scanning an object that is part of the user's **morning routine**.

These objects are selected during **onboarding** and can be modified at any time through the application's settings. Common examples include a **toothbrush**, **coffee mug**, **study materials**, **laptop**, **gym equipment**, or any other item that is consistently associated with the user's morning routine.

By requiring interaction with a ***real-world object***, Warden encourages users to **physically leave their bed** and begin their intended activities before regaining **unrestricted access** to their device. This creates a direct connection between ***productive behavior and reward***, making it easier for users to build **consistent morning habits**.

The **object scan** serves as a ***verification mechanism*** that the user has actively started their morning routine rather than simply bypassing the restriction. Once a **valid object** is detected, the remaining **WardenLock duration** is reduced, allowing users to complete their focus session earlier.

This approach was chosen to shift the user's attention away from the ***digital environment*** and toward ***real-world actions***. Rather than relying solely on **willpower**, Warden uses ***environmental cues*** and ***positive reinforcement*** to encourage productive behavior and establish ***morning momentum***.


</td>
<td width="35%" align="center">
<img alt="Morning Routine Scanner
" src="https://github.com/user-attachments/assets/b2b0b073-50ac-4fb4-8e13-19c38a4ae65a">
<br>
<em>Morning Routine Scanner
</em>
</td>
</tr>
</table>

### Allowed Apps

<table>
<tr>
<td width="65%">

The **Allowed Apps** section within the **WardenLock overlay** serves as both a **utility feature** and a **contingency mechanism**.

Users can add **essential applications** that may be required during a focus session, including **emergency and communication tools** such as Phone, Messages, Camera, and WhatsApp, as well as **productivity-oriented applications** such as web browsers and AI assistants like ChatGPT and Gemini.

To maintain the effectiveness of the **restriction system**, applications that are widely associated with **distraction and excessive engagement** cannot be added to the Allowed Apps list. According to a [DeskTime case study](https://desktime.com/blog/most-used-productive-unproductive-apps/), platforms such as **YouTube, Instagram, Facebook, and TikTok** consistently rank among the **most unproductive applications** in terms of time consumption and workplace distraction.

The **Allowed Apps list** is fully customizable. Applications that a user personally finds distracting can be removed at any time, even if they are permitted by default. For example, although **WhatsApp** is primarily a communication platform, the same [DeskTime case study](https://desktime.com/blog/most-used-productive-unproductive-apps/) reported it as one of the **most distracting applications** in both 2024 and 2025. Users who experience similar distractions can simply remove it from their Allowed Apps list.

To support this approach, Warden implements an **application-filtering algorithm** that automatically rejects specific categories of apps that are considered **unproductive in general**.

</td>
<td width="35%" align="center">
<img alt="Allowed Apps" src="https://github.com/user-attachments/assets/fc841de6-f386-4956-94af-881728a60d53">
<br>
<em>Allowed Apps</em>
</td>
</tr>
</table>

### Emergency Unlock

<table>
<tr>
<td width="65%">

Warden includes an **Emergency Unlock** mechanism to ensure that user safety and accessibility are never compromised during an active WardenLock session.

In situations where immediate access to the device is required, users can navigate to the **Allowed Apps** section and activate the **Emergency Unlock** option. This temporarily removes all restrictions and grants unrestricted access to the device for **five minutes**.

Unlike other unlocking methods, the Emergency Unlock is intentionally designed as a **fallback mechanism** rather than a routine method of bypassing restrictions. While WardenLock is designed to be highly resistant to circumvention, emergency situations require a balance between **focus enforcement** and **user safety**.

To reduce impulsive usage, the Emergency Unlock process includes a **30-second waiting period** before activation. This brief delay introduces a moment of reflection, helping users distinguish genuine emergencies from momentary urges to access distracting applications.

By combining accessibility with intentional friction, the Emergency Unlock system tries to ensure that users can always access their devices when necessary while preserving the effectiveness of the overall restriction system.

</td>
<td width="35%" align="center">
<img alt="Warden Emergency" src="https://github.com/user-attachments/assets/fcab78a5-1f11-4c5d-b8fa-8e89b945a362">
<br>
<em>Emergency Unlocks</em>
</td>
</tr>
</table>

### Statistics

<table>
<tr>
<td width="65%">
  
To provide users with ***clear insights into their device usage*** and enable ***data-driven habit improvement***, Warden displays a comprehensive set of usage statistics directly on the **Home Screen**.

Key metrics include:

* **Screen Time**
* **Screen Time Review**
* **Top Used Apps**
* **Device Unlocks**
* **Notifications Received**
* **Cumulative Weekly Screen Time**

These statistics are presented using a ***visually appealing yet easy-to-understand interface***. The design allows users to quickly interpret their usage patterns without requiring detailed analysis.

By making phone usage data readily available, Warden helps users develop a greater awareness of their digital habits. Users can identify patterns of excessive usage, monitor their progress over time, and evaluate the effectiveness of their focus routines.

The statistics also serve as a form of ***behavioral feedback***. During initial testing, users reported consciously reducing the number of device unlocks after observing high values on the **Unlocks Graph**. This suggests that increased visibility of usage patterns can encourage users to make more intentional decisions regarding their phone usage.

By transforming raw usage data into meaningful insights, Warden enables users to not only restrict distractions but also ***understand and improve the habits that create them***.

</td>
<td width="35%" align="center">
<img alt="Warden Statistics" src="https://github.com/user-attachments/assets/84fff5c9-f84a-43dd-977d-df45f30cd6e5">
<br>
<em>Statistics</em>
</td>
</tr>
</table>

## Screenshots

<table>
<tr>
<td><img src="https://github.com/user-attachments/assets/3ad47b3c-0263-4f94-bdfb-779ac1eb84cd" width="220"></td>
<td><img src="https://github.com/user-attachments/assets/694af787-1b06-47fd-856c-00a6d9410df0" width="220"></td>
<td><img src="https://github.com/user-attachments/assets/7ad2d015-1e87-4e4b-8174-0134e3f9ee78" width="220"></td>
</tr>
<tr>
<td><img src="https://github.com/user-attachments/assets/fa3c711c-d328-4beb-8ff9-7c542d08ac81" width="220"></td>
<td><img src="https://github.com/user-attachments/assets/13ce27d2-6746-49a4-a54c-92918ac273ea" width="220"></td>
<td><img src="https://github.com/user-attachments/assets/d5a1ed37-e2d0-4d34-a0ea-1b67762cbcaf" width="220"></td>
</tr>
</table>

<p align="center">
  <em>WardenLock</em>
</p>

<br><br>

<table>
<tr>
<td><img src="https://github.com/user-attachments/assets/c9ac5ce3-61a2-4a63-b44f-df15dc301660" width="220"></td>
<td><img src="https://github.com/user-attachments/assets/09028b2e-80b9-49d4-9b33-d5d3b2c71ee8" width="220"></td>
<td><img src="https://github.com/user-attachments/assets/4798e562-b01c-4269-bca8-60a2c667f2dd" width="220"></td>
</tr>
<tr>
<td><img src="https://github.com/user-attachments/assets/3dd843ea-3e89-4485-8a97-afd9009449ab" width="220"></td>
<td><img src="https://github.com/user-attachments/assets/2bb4fdd2-64d1-40a5-8a79-91b7219d184c" width="220"></td>
<td></td>
</tr>
</table>

<p align="center">
  <em>Home Screen</em>
</p>

## Technical Stack

### Mobile App
- Kotlin
- Jetpack Compose
- Android Studio
- Android SDK

### Cloud
- Fireabse Cloud Messaging
- Google AdMob
- Google ML Kit

### Version Control
- GitHub

## Architecture

All core application logic and system design were developed manually without the use of AI-generated code.

Several components, including the **object evaluation algorithm**, were specifically designed and optimized for Warden's use case and requirements.

As Warden is both a project and a product under active development, its source code remains private. Public documentation focuses on functionality rather than implementation details.

## Privacy
User data is processed and evaluated ***locally on the device*** wherever possible.

Warden does not knowingly share user data with **third-party services**. Information such as application usage statistics, screen time metrics, unlock counts, and object recognition results are processed directly on the user's device.

[Read Privacy Policy](https://wardenlanding.vercel.app/privacy.html)

## Roadmap

Warden is under active development, with several improvements and new features planned for future releases. Development progress may vary depending on academic commitments, but the project continues to be maintained and refined.

Further details regarding upcoming features will be shared as they become available.

## Status

**Actively Maintained**

