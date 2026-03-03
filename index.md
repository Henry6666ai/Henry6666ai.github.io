---
layout: default
title: Economics 101
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# 📈 Chapter 23: Measuring a Nation's Income

To understand how an economy is performing, we look at the **Gross Domestic Product (GDP)**. Whether you are looking at a single household or a whole nation, income must equal expenditure because every dollar spent by a buyer is a dollar of income for a seller.

---

## 🔍 What is GDP?
**Gross Domestic Product (GDP)** is the market value of all final goods and services produced within a country in a given period of time.

* **Market Value:** GDP uses market prices to measure the value of various goods.
* **Final Goods:** It includes only the value of final goods, not intermediate ones, to avoid double-counting.
* **Produced Within a Country:** It measures the value of production within a country's geographic borders.
* **In a Given Period:** Usually measured in a year or a quarter.

---

## 🧮 The Components of GDP
Economists divide GDP ($Y$) into four distinct categories of spending:

$$Y = C + I + G + NX$$



| Component | Description |
| :--- | :--- |
| **Consumption (C)** | Spending by households on goods and services, excluding new housing. |
| **Investment (I)** | Spending on capital equipment, inventories, structures, and new housing. |
| **Government Purchases (G)** | Spending on goods and services by local, state, and federal governments. |
| **Net Exports (NX)** | Spending on domestically produced goods by foreigners minus domestic spending on foreign goods. |

---

## ⚖️ Real vs. Nominal GDP
* **Nominal GDP:** The production of goods and services valued at **current prices**.
* **Real GDP:** The production of goods and services valued at **constant prices** (from a base year).

### The GDP Deflator
To measure the current level of prices relative to the level of prices in the base year:

$$\text{GDP Deflator} = \left( \frac{\text{Nominal GDP}}{\text{Real GDP}} \right) \times 100$$



---

## 📝 Chapter 23 Review Quiz

<div id="quiz-container" style="background-color: #f8f9fa; padding: 25px; border-radius: 10px; border: 1px solid #d1d5da; color: #24292e; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;">
  <p style="color: #586069;">Select your answers and click submit to see your results.</p>

  <div id="q1-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>1. If a consumer buys a brand-new house, which component of GDP does this fall under?</strong></p>
    <label style="display: block;"><input type="radio" name="q1" value="wrong"> Consumption (C)</label>
    <label style="display: block;"><input type="radio" name="q1" value="correct"> Investment (I)</label>
    <label style="display: block;"><input type="radio" name="q1" value="wrong"> Government Purchases (G)</label>
    <div id="feedback-q1" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q2-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>2. Which GDP measure should you use to see production volume ignoring price changes?</strong></p>
    <label style="display: block;"><input type="radio" name="q2" value="wrong"> Nominal GDP</label>
    <label style="display: block;"><input type="radio" name="q2" value="correct"> Real GDP</label>
    <label style="display: block;"><input type="radio" name="q2" value="wrong"> GDP Deflator</label>
    <div id="feedback-q2" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q3-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>3. If Nominal GDP is $600 and Real GDP is $500, what is the GDP Deflator?</strong></p>
    <label style="display: block;"><input type="radio" name="q3" value="wrong"> 83.3</label>
    <label style="display: block;"><input type="radio" name="q3" value="correct"> 120</label>
    <label style="display: block;"><input type="radio" name="q3" value="wrong"> 110</label>
    <div id="feedback-q3" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div style="text-align: center;">
    <button onclick="evaluateQuiz()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-weight: bold;">Submit Exam</button>
    <h3 id="score-display" style="margin-top: 20px;"></h3>
  </div>
</div>

<script>
function evaluateQuiz() {
  let score = 0;
  const answers = {
    q1: { correct: "correct", text: "Correct! New housing is Investment (I)." },
    q2: { correct: "correct", text: "Correct! Real GDP uses constant base-year prices." },
    q3: { correct: "correct", text: "Correct! (600 / 500) x 100 = 120." }
  };
  const hints = {
    q1: "Incorrect. New housing is specifically classed as Investment (I).",
    q2: "Incorrect. Real GDP is the measure adjusted for inflation.",
    q3: "Incorrect. Formula: (Nominal / Real) x 100."
  };

  for (let i = 1; i <= 3; i++) {
    const qName = 'q' + i;
    const selected = document.querySelector(`input[name="${qName}"]:checked`);
    const feedback = document.getElementById(`feedback-${qName}`);
    const box = document.getElementById(`${qName}-box`);

    if (selected) {
      if (selected.value === "correct") {
        score++;
        feedback.innerHTML = "✅ " + answers[qName].text;
        feedback.style.color = "#28a745";
        box.style.backgroundColor = "#e6ffed";
      } else {
        feedback.innerHTML = "❌ " + hints[qName];
        feedback.style.color = "#d73a49";
        box.style.backgroundColor = "#ffeef0";
      }
    }
  }
  document.getElementById('score-display').innerHTML = "Final Score: " + score + " / 3";
}
</script>
