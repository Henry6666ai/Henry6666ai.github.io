---
layout: default
title: Economics 101
---
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
| **Net Exports (NX)** | Spending on domestically produced goods by foreigners (exports) minus domestic spending on foreign goods (imports). |



---

## ⚖️ Real vs. Nominal GDP
If total spending rises from one year to the next, it’s either because the economy is producing more goods, or goods are being sold at higher prices.

* **Nominal GDP:** The production of goods and services valued at **current prices**.
* **Real GDP:** The production of goods and services valued at **constant prices** (from a base year).

> **The Goal:** Real GDP shows how the economy’s overall production changes over time, unaffected by price changes.

### The GDP Deflator
To measure the current level of prices relative to the level of prices in the base year, we use the GDP Deflator:

$$\text{GDP Deflator} = \left( \frac{\text{Nominal GDP}}{\text{Real GDP}} \right) \times 100$$

---

## 🌟 Is GDP a Good Measure of Well-being?
GDP is often considered the best single measure of the economic well-being of a society. While it doesn't directly measure health or education, nations with larger GDPs can afford better healthcare systems.

**What GDP excludes:**
1. Leisure time.
2. The quality of the environment.
3. Activity that takes place outside of markets (e.g., volunteer work).

---

<div id="quiz-container" style="background-color: #f8f9fa; padding: 25px; border-radius: 10px; border: 1px solid #d1d5da; color: #24292e; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif; margin-top: 30px;">
  <h2 style="margin-top: 0; color: #0366d6;">📝 Chapter 23 Review Quiz</h2>
  <p style="color: #586069;">Test your understanding of National Income and GDP components.</p>
  <hr style="border: 0; border-top: 1px solid #e1e4e8; margin: 20px 0;">

  <div id="q1-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px; transition: 0.3s;">
    <p><strong>1. If a consumer buys a brand-new house, which component of GDP does this fall under?</strong></p>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q1" value="wrong"> Consumption (C)</label>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q1" value="correct"> Investment (I)</label>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q1" value="wrong"> Government Purchases (G)</label>
    <div id="feedback-q1" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q2-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px; transition: 0.3s;">
    <p><strong>2. Which GDP measure should you use to see if an economy is actually producing more goods (ignoring price changes)?</strong></p>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q2" value="wrong"> Nominal GDP</label>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q2" value="correct"> Real GDP</label>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q2" value="wrong"> GDP Deflator</label>
    <div id="feedback-q2" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q3-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px; transition: 0.3s;">
    <p><strong>3. If Nominal GDP is $600 and Real GDP is $500, what is the GDP Deflator?</strong></p>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q3" value="wrong"> 83.3</label>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q3" value="correct"> 120</label>
    <label style="display: block; cursor: pointer;"><input type="radio" name="q3" value="wrong"> 110</label>
    <div id="feedback-q3" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div style="text-align: center; margin-top: 20px;">
    <button onclick="evaluateQuiz()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-size: 16px; font-weight: bold;">Submit Answers</button>
    <h3 id="score-display" style="margin-top: 20px;"></h3>
  </div>
</div>

<script>
function evaluateQuiz() {
  let score = 0;
  const total = 3;
  const answers = {
    q1: { correct: "correct", text: "Correct! New housing is categorized under Investment (I)." },
    q2: { correct: "correct", text: "Correct! Real GDP uses constant prices to measure volume." },
    q3: { correct: "correct", text: "Correct! (600 / 500) x 100 = 120." }
  };
  
  const explanations = {
    q1: "Incorrect. While most household spending is Consumption, new housing is specifically classed as Investment (I).",
    q2: "Incorrect. Nominal GDP includes price changes; Real GDP is the measure adjusted for inflation.",
    q3: "Incorrect. The formula is (Nominal / Real) x 100. So, (600/500) * 100 = 120."
  };

  for (let i = 1; i <= total; i++) {
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
        box.style.borderLeft = "5px solid #28a745";
      } else {
        feedback.innerHTML = "❌ " + explanations[qName];
        feedback.style.color = "#d73a49";
        box.style.backgroundColor = "#ffeef0";
        box.style.borderLeft = "5px solid #d73a49";
      }
    } else {
      feedback.innerHTML = "⚠️ Please select an answer.";
      feedback.style.color = "#f66a0a";
    }
  }

  const scoreDisplay = document.getElementById('score-display');
  scoreDisplay.innerHTML = "Total Score: " + score + " / " + total;
  scoreDisplay.style.color = score === total ? "#28a745" : "#24292e";
}
</script>
