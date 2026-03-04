---
layout: default
title: Chapter 25 - Production and Growth
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# 🚀 Module: Economic Growth & Productivity

Why do some countries enjoy a high standard of living while others struggle? The answer lies in **productivity**. A nation’s standard of living depends on its ability to produce goods and services.

---

## 🛠️ The Pillars of Productivity
Productivity is the quantity of goods and services produced from each unit of labor input. It is determined by four key factors:



* **Physical Capital:** The stock of equipment and structures used to produce goods and services (e.g., tools, factories).
* **Human Capital:** The knowledge and skills workers acquire through education, training, and experience.
* **Natural Resources:** Inputs provided by nature, such as land, rivers, and mineral deposits.
* **Technological Knowledge:** Society’s understanding of the best ways to produce goods and services.

---

## 📈 Economic Growth & Public Policy

### 1. Saving and Investment
To raise future productivity, a society must invest more in capital. This requires a trade-off: to invest more today, we must **consume less and save more** of our current income.

### 2. The Catch-up Effect
It is easier for a country to grow fast if it starts out relatively poor. This occurs because of **diminishing returns**: in a rich country, more capital adds little to productivity; in a poor country, a little capital goes a long way.



### 3. Investment from Abroad
| Investment Type | Definition |
| :--- | :--- |
| **Foreign Direct Investment (FDI)** | Capital investment owned and operated by a foreign entity. |
| **Foreign Portfolio Investment** | Investment financed with foreign money but operated by domestic residents. |

### 4. Education and Health
* **Education:** Investment in human capital. A major challenge for poor countries is "brain drain."
* **Health:** Healthier workers are more productive, creating a virtuous circle of growth.

---

## 🏛️ Institutions and Growth

* **Property Rights & Political Stability:** Essential for the price system to work; people must know their investments are safe from theft or corruption.
* **Free Trade:** Outward-oriented policies are generally better for growth than inward-oriented (protectionist) ones.
* **Research and Development:** Knowledge is a public good. Governments encourage R&D through grants and the patent system.

---

## 📝 Knowledge Check: Multiple Choice

<div id="quiz-container" style="background-color: #f8f9fa; padding: 25px; border-radius: 10px; border: 1px solid #d1d5da; color: #24292e; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;">
  
  <div id="q1-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>1. Which of the following is considered "human capital"?</strong></p>
    <label style="display: block;"><input type="radio" name="q1" value="A"> A) A new automated assembly line</label>
    <label style="display: block;"><input type="radio" name="q1" value="B"> B) Knowledge gained from a training course</label>
    <label style="display: block;"><input type="radio" name="q1" value="C"> C) A large deposit of copper</label>
    <div id="feedback-q1" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q2-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>2. What is the "catch-up effect"?</strong></p>
    <label style="display: block;"><input type="radio" name="q2" value="A"> A) Rich countries growing faster due to tech</label>
    <label style="display: block;"><input type="radio" name="q2" value="B"> B) Government catching tax evaders</label>
    <label style="display: block;"><input type="radio" name="q2" value="C"> C) Poor countries growing faster than rich ones</label>
    <div id="feedback-q2" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q3-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>3. A US company opening and operating a factory in Vietnam is:</strong></p>
    <label style="display: block;"><input type="radio" name="q3" value="A"> A) Foreign Portfolio Investment</label>
    <label style="display: block;"><input type="radio" name="q3" value="B"> B) Human Capital Investment</label>
    <label style="display: block;"><input type="radio" name="q3" value="C"> C) Foreign Direct Investment</label>
    <div id="feedback-q3" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q4-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>4. Why is political stability vital for economic growth?</strong></p>
    <label style="display: block;"><input type="radio" name="q4" value="A"> A) It ensures the gov can print money</label>
    <label style="display: block;"><input type="radio" name="q4" value="B"> B) It protects property rights</label>
    <label style="display: block;"><input type="radio" name="q4" value="C"> C) It prevents price changes</label>
    <div id="feedback-q4" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div style="text-align: center;">
    <button onclick="checkQuiz25()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-weight: bold;">Submit & View Correct Answers</button>
    <h3 id="score-display" style="margin-top: 20px;"></h3>
  </div>
</div>

<script>
function checkQuiz25() {
  let score = 0;
  const total = 4;
  const keys = {
    q1: { ans: "B", note: "Correct! Human capital refers to skills and knowledge." },
    q2: { ans: "C", note: "Correct! Poor countries grow faster because initial capital has a larger impact." },
    q3: { ans: "C", note: "Correct! Ownership and operation by a foreign entity = FDI." },
    q4: { ans: "B", note: "Correct! Property rights give people the incentive to save and invest." }
  };

  for (let i = 1; i <= total; i++) {
    const qName = 'q' + i;
    const selected = document.querySelector(`input[name="${qName}"]:checked`);
    const feedback = document.getElementById(`feedback-${qName}`);
    const box = document.getElementById(`${qName}-box`);

    if (selected) {
      if (selected.value === keys[qName].ans) {
        score++;
        feedback.innerHTML = "✅ " + keys[qName].note;
        feedback.style.color = "#28a745";
        box.style.backgroundColor = "#e6ffed";
      } else {
        feedback.innerHTML = "❌ Wrong. The correct answer was " + keys[qName].ans + ". " + keys[qName].note.replace("Correct! ", "");
        feedback.style.color = "#d73a49";
        box.style.backgroundColor = "#ffeef0";
      }
    }
  }
  document.getElementById('score-display').innerHTML = "Your Score: " + score + " / " + total;
}
</script>

---
[⬅ Back to Chapter 24 (Inflation)](index24.html) | [🏠 Home](index.html)
