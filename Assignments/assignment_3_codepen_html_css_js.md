[![Learn and Help Logo](https://www.learnandhelp.com/images/supported_by/learn_n_help_logo.png)](https://www.learnandhelp.com)  
***Empowering Minds, Inspiring Generosity!***  
[**www.learnandhelp.com**](https://www.learnandhelp.com)

# 🌟 Code for Good — Assignment 3

## Community Helper Mini-Page: HTML + CSS + JavaScript in CodePen

| | |
| --- | --- |
| **Points** | 25 |
| **Due** | **10/17/26** |
| **Tool** | [CodePen](https://codepen.io) (free account) |
| **Submit to** | Google Classroom |

---

## 🎯 Goal

Build a small, working web page in **CodePen** that uses all three core web languages together:

- **HTML** builds the structure.
- **CSS** controls how it looks.
- **JavaScript** makes it respond when someone clicks or types.

Then record a short **video demo** where you show your page working and explain your code in your own words.

---

## 📚 Before You Start

Use the Week 3 and Week 4 resources:

- [HTML Forms Playbook](https://github.com/sjasthi/ICS325-Web-Application-Development/blob/main/HTML/html-forms-playbook-quiz.html)
- [CSS Playbook](https://github.com/sjasthi/ICS325-Web-Application-Development/blob/main/CSS/css_playbook_quiz.html)
- [CSS One Pager](https://github.com/sjasthi/ICS325-Web-Application-Development/blob/main/CSS/css-in-10-points-A4.png)
- [W3Schools CSS](https://www.w3schools.com/css/) and [W3Schools JavaScript](https://www.w3schools.com/js/)

**Set up CodePen:**

1. Go to [codepen.io](https://codepen.io) and create a free account.
2. Click **Start Coding** to open a new Pen. You will see three panes: HTML, CSS, and JS.
3. Click **Save** often. Your Pen must be **public** (or at least viewable by anyone with the link) so it can be graded.
4. Give the Pen a clear title, for example `Donation Goal Tracker - Your Name`.

---

## 🛠️ What You Will Build: A "Goal Tracker" for an Organization You Care About

Pick a real or imaginary organization (a food shelf, animal shelter, school club, etc.) and build a one-page **Goal Tracker**. Visitors enter an amount (dollars, volunteer hours, or items collected), click a button, and the page updates a running total and progress message.

You may choose a different idea (for example a volunteer sign-up counter or a "pledge" wall) **if you check with the instructor first** and it meets every requirement below.

---

## ✅ Requirements

### Part 1: HTML (5 points)

Your **HTML pane** must include all of the following:

- [ ] A `<header>` containing an `<h1>` with the organization's name
- [ ] A short `<p>` paragraph describing the organization and the goal (for example, "Help us collect 500 cans by December!")
- [ ] A `<main>` section that holds the tracker
- [ ] A `<label>` connected to an `<input type="number">` (use matching `for` and `id`)
- [ ] A `<button>` with the text "Add"
- [ ] An element (such as a `<span>` or `<p>`) that displays the **current total**, with an `id` so JavaScript can find it
- [ ] A `<ul>` list with **at least 3 items** (for example, "Ways to help" or "Recent contributions")
- [ ] A `<footer>` with your name

### Part 2: CSS (6 points)

Your **CSS pane** must include all of the following. Add a short comment (`/* ... */`) next to each one so it is easy to find.

- [ ] An **element selector** (for example `h1 { ... }`)
- [ ] A **class selector** (for example `.card { ... }`)
- [ ] An **id selector** (for example `#total { ... }`)
- [ ] A **grouping or descendant selector** (for example `h1, h2 { ... }` or `.card p { ... }`)
- [ ] **Box model**: use `padding`, `margin`, and `border` on at least one element, and include `box-sizing: border-box;`
- [ ] **Text and color**: set `font-family`, `color`, and `background-color`
- [ ] **Flexbox**: use `display: flex;` with `justify-content` or `gap` (for example, to lay out the input and button in a row, or to build a navigation bar)
- [ ] A **`:hover` style** on the button (for example, change its background color)

**Design tip:** choose 2 or 3 colors and stick with them. A clean, simple page earns the same points as a fancy one.

### Part 3: JavaScript (6 points)

Your **JS pane** must include all of the following. Add a short comment above each one explaining what it does.

- [ ] A **variable** that stores the running total (start at `0`) and a variable for the goal (for example, `const goal = 500;`)
- [ ] A **function** that runs when the button is clicked
- [ ] An **event listener** (`addEventListener('click', ...)`) or an `onclick` attached to the button
- [ ] Code that **reads the number** the user typed into the input
- [ ] An **`if` statement** that checks the input is valid (for example, a number greater than 0). If it is not, show a friendly error message instead of adding.
- [ ] Code that **updates the page** by changing the text of your total element (`textContent`) after each click
- [ ] A **progress message** that changes using `if / else` (for example, "Just getting started!", "Halfway there!", "Goal reached! Thank you!")

**Starter hint (not the full answer):**

```js
const goal = 500;
let total = 0;

const button = document.getElementById("addBtn");
button.addEventListener("click", function () {
  // 1. Read the input
  // 2. Check it is valid with an if statement
  // 3. Add it to total
  // 4. Update the page with textContent
  // 5. Show a progress message
});
```

### Part 4: Video Demonstration (6 points)

Record a video that is **2 to 4 minutes** long. Your face does not have to be on camera, but we must be able to **hear you clearly** and **see your screen**.

Your video must:

1. **Introduce** yourself and your organization (15-20 seconds).
2. **Demo the page working**: type a valid number, click the button, and show the total and message changing. Then show the **error case** (for example, an empty or negative number).
3. **Walk through your HTML** and point out the label/input, the button, and the element that shows the total.
4. **Walk through your CSS** and point out at least **three** of the required items (for example, the class selector, box-sizing, and Flexbox) and show what changes when you edit one value live.
5. **Walk through your JavaScript** and explain, in your own words, what the function does and how the `if` statement works.
6. **Reflect (20-30 seconds)**: share one thing that was hard, and one thing you learned.

**How to record (free options):**

- **Loom** (loom.com) or **Screencastify** (Chrome extension)
- **Zoom**: start a meeting by yourself, share your screen, and record
- **Windows**: Xbox Game Bar (press `Win + G`)
- **Mac**: QuickTime Player, then File > New Screen Recording
- **Phone**: a screen recording plus voice works too

**How to share:** upload to YouTube as **Unlisted**, or to Google Drive with the sharing set to **"Anyone with the link can view."** Open the link in a private/incognito window to confirm it works before you submit.

### Part 5: Submission and AI Prompt Log (2 points)

In Google Classroom, submit:

1. Your **CodePen link** (public)
2. Your **video link**
3. A short **AI Prompt Log** (a few sentences in the text box or a document): paste **two prompts** you used with GitHub Copilot or Claude while working on this assignment. At least **one** must use the **structured prompt template** (Role, Task, Context, Format, Constraints). Add one sentence on how the answer helped.

---

## 📊 Grading Rubric (25 points)

| Category | Points | What earns full credit |
| --- | :---: | --- |
| **HTML** | 5 | All 8 required elements are present and sensibly used |
| **CSS** | 6 | All 8 required items are present; the page looks clean and consistent |
| **JavaScript** | 6 | The page works: valid input updates the total, invalid input shows a friendly error, and the message changes with progress |
| **Video** | 6 | 2-4 minutes, clear audio, covers all 6 video points, and the explanations are in your own words |
| **Submission and AI Prompt Log** | 2 | Both links work, and 2 prompts are included (1 structured) |
| **Total** | **25** | |

**Partial credit:** each category is graded on how many of its checklist items are complete and working.

---

## 🤖 Using AI (GitHub Copilot or Claude) on This Assignment

You are encouraged to use GitHub Copilot or Claude to **learn**: ask it to explain an error, show an example, or review your code. But the work you submit must be **yours**, and you must understand it. If your AI tool writes code for you, read it, test it, and be ready to **explain every line in your video**. A video where the code can't be explained will lose points, even if the code works.

**Prompts to try:**

- "My button click does nothing. Here is my code: [paste]. Explain what's wrong in 3 simple steps."
- Act as a **JavaScript tutor**. Task: **explain what `addEventListener` does**. Context: **I know HTML and CSS but I'm new to JavaScript**. Format: **a short explanation and one small example with comments**. Constraints: **under 150 words, no jargon**.
- Act as a **code reviewer**. Task: **check my CSS against this list** [paste the CSS requirements]. Context: **I'm a beginner**. Format: **a table with Requirement | Done? | Fix**. Constraints: **under 200 words**.

---

## 🧰 Troubleshooting Tips

- **Nothing happens when I click:** make sure the button's `id` in HTML exactly matches the `id` in your JavaScript (spelling and capital letters count).
- **My total shows `NaN` or joins numbers like "1020":** input values are text. Convert with `Number(input.value)`.
- **My CSS isn't applying:** check for a missing `;`, `}`, or a typo in the class name. Remember a class uses `.` and an id uses `#`.
- **Open the browser console** (in CodePen, click **Console** at the bottom left) to see JavaScript error messages.
- **Don't wait until the last day.** Build one part at a time: HTML first, then CSS, then JavaScript. Save after each step.

---

## 📌 Summary

| Item | Details |
| --- | --- |
| Assignment | Community Helper Mini-Page (HTML + CSS + JavaScript in CodePen) |
| Points | 25 |
| Due | **10/18** |
| Submit | CodePen link + video link + AI Prompt Log, in Google Classroom |
