---
layout: default
title: Chapter 25 - Production and Growth
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# 🚀 Chapter 25: Production and Growth

Economic growth varies significantly across the globe. We measure these differences using **Real GDP per person**, which serves as a primary indicator of the standard of living in a country.

---

## Introduction to Economic Growth
* **Variation:** Living standards vary widely from country to country.
* **Growth Rate:** Measures how rapidly real GDP per person grows in a typical year.

---

## The Power of Productivity
Productivity is the quantity of goods and services produced from each unit of labor input. 

> **Core Principle:** An economy’s income is the economy’s output. If productivity grows, living standards grow.



### The Four Determinants
1.  **Physical Capital:** The stock of equipment and structures used to produce goods.
2.  **Human Capital:** The knowledge and skills workers acquire through education and experience.
3.  **Natural Resources:** Inputs provided by nature, such as land and minerals.
4.  **Technological Knowledge:** Society’s understanding of the best ways to produce goods.

---

## Public Policy and Investment

### Saving and Investment
To raise future productivity, a society must invest more current resources in the production of capital. This requires a trade-off: to have more capital in the future, we must consume less today.

### Diminishing Returns and the Catch-up Effect
* **Diminishing Returns:** As the stock of capital rises, the extra output produced from an additional unit of capital falls.
* **Catch-up Effect:** Countries that start off poor tend to grow more rapidly than countries that start off rich.

<div style="text-align: center; margin: 25px 0;">
  <img src="production-function.png" alt="Production Function and Diminishing Returns" style="max-width: 90%; border-radius: 8px; border: 1px solid #ddd; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <p style="color: #6a737d; font-style: italic; font-size: 0.9em; margin-top: 10px;">
    Figure 1: The Production Function. Note how the curve flattens as capital per worker increases due to diminishing returns.
  </p>
</div>

### Investment from Abroad
Investment doesn't just come from domestic residents.

| Investment Type | Description |
| :--- | :--- |
| **Foreign Direct Investment (FDI)** | Capital investment owned and operated by a foreign entity. |
| **Foreign Portfolio Investment** | Investment financed with foreign money but operated by domestic residents. |

---

## 📝 Practice Quiz

<div id="quiz-container" style="background-color: #f8f9fa; padding: 25px; border-radius: 10px; border: 1px solid #d1d5da; color: #24292e; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;">
  
  <div id="q1-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>1. Which determinant refers to "knowledge and skills workers acquire"?</strong></p>
    <label style="display: block;"><input type="radio" name="q1" value="A"> A) Physical Capital</label>
    <label style="display: block;"><input type="radio" name="q1" value="B"> B) Human Capital</label>
    <label style="display: block;"><input type="radio" name="q1" value="C"> C) Natural Resources</label>
    <div id="feedback-q1" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q2-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>2. The "catch-up effect" suggests that:</strong></p>
    <label style="display: block;"><input type="radio" name="q2" value="A"> A) Rich countries grow faster</label>
    <label style="display: block;"><input type="radio" name="q2" value="B"> B) Poor countries tend to grow more rapidly</label>
    <label style="display: block;"><input type="radio" name="q2" value="C"> C) Education is the only way to grow</label>
    <div id="feedback-q2" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div style="text-align: center;">
    <button onclick="checkQuiz25()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-weight: bold;">Check Answers</button>
    <h3 id="score-display" style="margin-top: 20px;"></h3>
  </div>
</div>

<script>
function checkQuiz25() {
  let score = 0;
  const solutions = {
    q1: { ans: "B", txt: "Human capital refers to the education and skills of the labor force." },
    q2: { ans: "B", txt: "Poor countries see higher returns on initial capital investments." }
  };

  for (let i = 1; i <= 2; i++) {
    const qName = 'q' + i;
    const selected = document.querySelector(`input[name="${qName}"]:checked`);
    const feedback = document.getElementById(`feedback-${qName}`);
    const box = document.getElementById(`${qName}-box`);

    if (selected) {
      if (selected.value === solutions[qName].ans) {
        score++;
        feedback.innerHTML = "✅ Correct!";
        feedback.style.color = "#28a745";
        box.style.backgroundColor = "#e6ffed";
      } else {
        feedback.innerHTML = "❌ Wrong. The correct answer is " + solutions[qName].ans + ". " + solutions[qName].txt;
        feedback.style.color = "#d73a49";
        box.style.backgroundColor = "#ffeef0";
      }
    }
  }
  document.getElementById('score-display').innerHTML = "Final Score: " + score + " / 2";
}
</script>

---
[⬅ Back to Chapter 24](index24.html) | [🏠 Home](index.html)
