<p align="center"><img src="https://www.learnandhelp.com/images/supported_by/learn_n_help_logo.png" alt="Learn and Help Logo" width="220"><br><strong><em>Empowering Minds, Inspiring Generosity!</em></strong><br><a href="https://www.learnandhelp.com">www.learnandhelp.com</a></p>

# Document Object Model (DOM)

Code for Good · Week 6 · Prerequisite: HTML, CSS, and Week 5 JavaScript basics.

## Learning goals

Select elements, update text and classes, read inputs, and create or remove elements. Explain how JavaScript changes the browser’s current document.

## From Python to the browser

Python variables hold objects; JavaScript variables can hold references to DOM elements. A Python list is not a DOM NodeList, but you can loop over both. `print()` and `console.log()` show diagnostic output; updating `textContent` changes the visible page. DOM edits are temporary unless your application explicitly saves data.

## Sample HTML

```html
<h2 id="mission">Code for Good</h2>
<section id="card"><p id="status">Ready to help</p>
<label>Donation amount <input id="amount" type="number" value="25"></label>
<ul id="causes"><li class="cause">Donate books</li><li class="cause">Teach coding</li></ul>
<a id="helpLink" href="#">Learn more</a></section>
```

Use each example below with this sample. Start fresh for each experiment. For a local HTML file, put JavaScript inside `<script>` just before `</body>`. For an external file use `<script defer src="app.js"></script>` in the head.

## 1. Meet the DOM

The browser turns HTML into a tree of objects. JavaScript uses this tree to update the page. Elements, text, and comments are nodes. The DOM is a browser API, not the JavaScript language itself.

```javascript
console.log(document.title);
```

**Predict → Run → Modify → Explain:** Inspect the Elements panel. Expand body and find the heading.

## 2. Select one element

Use a CSS selector with querySelector. It returns the first match, or null if no element matches. getElementById takes an ID without #.

```javascript
const heading = document.querySelector("#mission");
heading.textContent = "Learning changes lives";
```

**Predict → Run → Modify → Explain:** Select #status and change its message.

## 3. Select many elements

querySelectorAll returns a static NodeList. Use for...of to work with every match; it is not a single element.

```javascript
for (const item of document.querySelectorAll(".cause")) {
  item.classList.add("highlight");
}
```

**Predict → Run → Modify → Explain:** Change the selector to li. Which items change?

## 4. Change text safely

textContent inserts plain text. innerHTML parses markup; avoid using it for user input. Replacing textContent also replaces existing child content.

```javascript
document.querySelector("#status").textContent = "Books delivered!";
```

**Predict → Run → Modify → Explain:** Try the text <strong>Thank you</strong> with textContent. Is it bold?

## 5. Read input values

An input uses .value, which is a string. Use Number when you need arithmetic. An empty string converts to 0; validation comes next week.

```javascript
const amount = Number(document.querySelector("#amount").value);
document.querySelector("#status").textContent = `Total: ${amount + 10}`;
```

**Predict → Run → Modify → Explain:** Enter 25. Predict the result before running.

## 6. Change classes and styles

Prefer classList for reusable CSS. add, remove, and toggle change class membership. Inline style uses camelCase property names.

```javascript
const card = document.querySelector("#card");
card.classList.toggle("highlight");
card.style.borderRadius = "20px";
```

**Predict → Run → Modify → Explain:** Run toggle twice. Explain why the appearance changes back.

## 7. Update attributes

setAttribute changes HTML attributes; properties also expose many values. Use hidden to show or hide content.

```javascript
const link = document.querySelector("#helpLink");
link.setAttribute("href", "https://www.learnandhelp.com");
link.textContent = "Visit Learn and Help";
document.querySelector("#status").hidden = false;
```

**Predict → Run → Modify → Explain:** Hide #status using its hidden property, then show it.

## 8. Create and append

createElement makes a detached element. Set its text, then append it to a parent so it appears.

```javascript
const item = document.createElement("li");
item.textContent = "Support a school library";
item.classList.add("cause");
document.querySelector("#causes").append(item);
```

**Predict → Run → Modify → Explain:** Run twice. Why are there two new items?

## 9. Traverse and remove

parentElement, children, and nextElementSibling follow element relationships. remove detaches an element. Check for a missing element before using it.

```javascript
const first = document.querySelector("#causes li");
if (first) {
  console.log(first.parentElement.id);
  first.remove();
}
```

**Predict → Run → Modify → Explain:** Remove items until the list is empty. Why does the guard matter?

## 10. Run after the HTML exists

Place a script at the end of body, or use defer on an external script. A premature selection may return null. DOM edits affect the current page; reload restores the source unless data is saved.

```javascript
const status = document.querySelector("#status");
if (status) {
  status.textContent = "Ready to make a difference!";
}
```

**Predict → Run → Modify → Explain:** Reload the page. Did your temporary DOM changes persist?

## Integrated practice: Library campaign

Build a campaign card from the sample HTML. Change the heading, calculate a donation total, add a cause, highlight all causes, and safely remove the first cause. Capture before/after screenshots and explain two changes. Use a CSS `.highlight` class of your own.

For an introductory click demonstration, place this after the markup and your `updateCampaign` function:

```javascript
// Add <button id="update" type="button">Update campaign</button> to the HTML.
function updateCampaign() {
  const amount = Number(document.querySelector("#amount").value);
  document.querySelector("#status").textContent = `Total: ${amount + 10}`;
}
document.querySelector("#update").addEventListener("click", updateCampaign);
```

This listener calls the function when clicked. Events and input validation are the focus of Week 7. This preview assumes a valid numeric value; production donation forms also need validation and server-side checks.

## Common mistakes

| Symptom | Check |
| --- | --- |
| Cannot read properties of null | Selector spelling and script timing |
| Only one item changes | querySelector selects only the first match |
| 20 + 5 becomes 205 | Convert the input string using Number |
| Newly created item is invisible | Append it to an existing parent |
| Typed markup unexpectedly becomes HTML | Use textContent for plain text |
| Changes vanish after reload | DOM updates do not rewrite source files |

## Resources

- [Interactive 10 Points](document-object-model-in-10-points.html)
- [One-pager](docuemnt-object-model-one-pager.png)
- [Playbook and 10-question quiz](document-object-model-playbook-and-quiz.html)
- [MDN: DOM scripting](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Scripting/DOM_scripting)
- [MDN: querySelector](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)
- [MDN: textContent](https://developer.mozilla.org/en-US/docs/Web/API/Node/textContent)

Download HTML files and open them in a browser; GitHub’s file view shows source code.
