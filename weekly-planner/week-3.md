<p align="center">
  <img src="https://www.learnandhelp.com/images/supported_by/learn_n_help_logo.png"
       alt="Learn and Help Logo"
       width="220">
  <br>
  <strong><em>Empowering Minds, Inspiring Generosity!</em></strong>
  <br>
  <a href="https://www.learnandhelp.com"><strong>www.learnandhelp.com</strong></a>
</p>

# 🌟 Code for Good — Week 3

## HTML Forms and Structured Prompt Templates

---

## 📚 Topics & Resources

1. **HTML Forms in 10 Points** (interactive: edit the code and see the result instantly)
   [html-forms-in-10-points.html](https://github.com/sjasthi/ICS325-Web-Application-Development/blob/main/HTML/html-forms-in-10-points.html)

2. **HTML Forms One Pager** (print it or keep it open while you code)
   [html-forms-in-10-points-A4.png](https://github.com/sjasthi/ICS325-Web-Application-Development/blob/main/HTML/html-forms-in-10-points-A4.png)

3. **HTML Forms Playbook**
   [html-forms-playbook-quiz.html](https://github.com/sjasthi/ICS325-Web-Application-Development/blob/main/HTML/html-forms-playbook-quiz.html)
   - Inputs & Labels
   - Choices (radio, checkbox, select, textarea)
   - Validation Basics (`required`, `min`/`max`, `pattern`)
   - Sending Data (`name`, `action`, GET vs POST)
   - Structured Prompt Templates

4. **HTML Forms Tutorial at W3Schools**
   [w3schools.com/html/html_forms.asp](https://www.w3schools.com/html/html_forms.asp)

5. **Structured Prompt Templates**
   Last week we learned prompt engineering basics. This week we make our prompts **structured**: fill in the same five parts every time, just like filling in a form.

   | Part | Question it answers | Example |
   |------|---------------------|---------|
   | 🎭 **Role** | Who should the AI act as? | "Act as a patient coding tutor." |
   | 🎯 **Task** | What exactly do you want? | "Explain GET vs POST." |
   | 📚 **Context** | What background does it need? | "I'm in 8th grade and just learned HTML forms." |
   | 📋 **Format** | How should the answer look? | "A bulleted list with one code example." |
   | 📏 **Constraints** | What are the limits or rules? | "Under 150 words. No jargon." |

   **Template (copy and fill in the blanks):**
   ```text
   Act as [role].
   Task: [what you want].
   Context: [background the AI needs].
   Format: [list / table / steps / code with comments].
   Constraints: [length, level, what to include or avoid].
   ```

6. **In-Class Exercise — HTML Forms Prompts to Try**

   Try each prompt as a one-liner first, then rewrite it using the structured template above. Compare the two answers.

   **Tier 1 — Form Basics**
   - "Explain what the `<form>`, `<label>`, and `<input>` tags do, in simple terms."
   - "Show me two ways to connect a `<label>` to an `<input>`, and explain why labels matter for accessibility."
   - "Show me 10 different `<input>` types with one example each."
   - "What is the difference between `placeholder` and `value`?"

   **Tier 2 — Choices and Grouping**
   - "When should I use radio buttons, checkboxes, or a `<select>` dropdown? Give an example of each."
   - "Why do radio buttons in the same group need the same `name`?"
   - "Create a volunteer sign-up form that uses `<fieldset>` and `<legend>` to group the questions."
   - "What is the difference between `readonly` and `disabled`?"

   **Tier 3 — Validation Basics**
   - "Show me how to use `required`, `minlength`, `maxlength`, `min`, and `max` on form fields."
   - "Write a `pattern` that accepts only a 5-digit ZIP code, and explain how it works."
   - "Why can't I rely only on HTML validation? What could a user do to bypass it?"
   - "What is the difference between client-side and server-side validation?"

   **Tier 4 — Structured Prompts (use the template!)**
   - Act as a **web accessibility reviewer**. Task: **review my contact form** (paste your HTML). Context: **it is for a local food shelf**. Format: **a table with Problem | Why it matters | Fix**. Constraints: **under 200 words**.
   - Act as a **senior web developer**. Task: **create a donation form** for a nonprofit. Context: **donors choose an amount, a frequency, and leave an optional message**. Format: **HTML with comments**. Constraints: **use labels, validation, and `method="post"`**.
   - Act as a **coding tutor**. Task: **explain what happens after I click Submit**. Context: **I know HTML but have not learned PHP yet**. Format: **5 numbered steps**. Constraints: **no more than 2 sentences per step**.
   - Write your **own** structured prompt that asks Claude to build a form for an organization you care about.

7. **HTML Forms Quiz (10 Points)** — Due **10/2**
   [html-forms-playbook-quiz.html](https://github.com/sjasthi/ICS325-Web-Application-Development/blob/main/HTML/html-forms-playbook-quiz.html) (open the ✅ Quiz tab, then screenshot your score and submit it to Google Classroom)

8. **Assignment 2: About Me** — Due **10/9**
   [assignment_2_about_me.md](https://github.com/sjasthi/code4good/blob/main/Assignments/assignment_2_about_me.md)

---

## 📌 Summary

| # | Topic                                  | Due   |
|---|----------------------------------------|-------|
| 1 | HTML Forms in 10 Points                | —     |
| 2 | HTML Forms One Pager                   | —     |
| 3 | HTML Forms Playbook                    | —     |
| 4 | HTML Forms Tutorial at W3Schools       | —     |
| 5 | Structured Prompt Templates            | —     |
| 6 | In-Class Exercise (HTML Forms Prompts) | —     |
| 7 | HTML Forms Quiz (10 pts)               | 10/2  |
| 8 | Assignment 2: About Me                 | 10/9  |
