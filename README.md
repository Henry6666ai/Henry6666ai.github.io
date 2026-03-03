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

<div id="quiz-container" style="background-color: #fdfdfd; padding: 25px; border-radius: 12px; border: 1px solid #e1e4e8; color: #24292e; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;">
  <h3 style="margin-top: 0;">🧠 Economics Knowledge Check</h3>
  <p style="font-size: 0.9em; color: #586069;">Select your answers and click submit to see your results.</p>
  <hr style="border: 0; border-top: 1px solid #eaecef; margin: 20px 0;">

  <div id="q1-area" style="margin-bottom: 25px; padding: 10px; border-radius: 6px;">
    <p><strong>1. Which component of GDP includes the purchase of a brand-new home?</strong></p>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q1" value="wrong"> Consumption (C)</label>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q1" value="correct"> Investment (I)</label>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q1" value="wrong"> Government Purchases (G)</label>
    <span id="feedback-q1" style="font-weight: bold; display: block; margin-top: 5px;"></span>
  </div>

  <div id="q2-area" style="margin-bottom: 25px; padding: 10px; border-radius: 6px;">
    <p><strong>2. Which measure of GDP is adjusted for inflation (valued at constant prices)?</strong></p>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q2" value="wrong"> Nominal GDP</label>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q2" value="correct"> Real GDP</label>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q2" value="wrong"> GDP Deflator</label>
    <span id="feedback-q2" style="font-weight: bold; display: block; margin-top: 5px;"></span>
  </div>

  <div id="q3-area" style="margin-bottom: 25px; padding: 10px; border-radius: 6px;">
    <p><strong>3. Why is the purchase of flour by a baker excluded from GDP?</strong></p>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q3" value="wrong"> It is a service, not a good.</label>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q3" value="correct"> It is an intermediate good (to avoid double-counting).</label>
    <label style="display: block; margin-bottom: 5px;"><input type="radio" name="q3" value="wrong"> It is produced outside the country.</label>
    <span id="feedback-q3" style="font-weight: bold; display: block; margin-top: 5px;"></span>
  </div>

  <div style="text-align: center; margin-top: 30px;">
    <button onclick="checkAnswers()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 30px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 1rem;">Submit Exam</button>
    <p id="total-score" style="margin-top: 20px; font-weight: bold; font-size: 1.3em;"></p>
  </div>
</div>

<script>
function checkAnswers() {
  let score = 0;
  const questions = [
    {id: 'q1', correct: 'Investment (I)'},
    {id: 'q2', correct: 'Real GDP'},
    {id: 'q3', correct: 'An intermediate good'}
  ];

  questions.forEach((q, index) => {
    const num = index + 1;
    const selected = document.querySelector(`input[name="q${num}"]:checked`);
    const feedback = document.getElementById(`feedback-q${num}`);
    const area = document.getElementById(`q${num}-area`);

    if (selected) {
      if (selected.value === "correct") {
        score++;
        feedback.innerHTML = "✓ Correct!";
        feedback.style.color = "#28a745";
        area.style.backgroundColor = "#f0fff4"; // Light green background
      } else {
        feedback.innerHTML = "✗ Incorrect. The correct answer is: " + q.correct;
        feedback.style.color = "#d73a49";
        area.style.backgroundColor = "#ffeef0"; // Light red background
      }
    } else {
      feedback.innerHTML = "⚠ Please select an answer.";
      feedback.style.color = "#f66a0a";
    }
  });

  const finalResult = document.getElementById('total-score');
  finalResult.innerHTML = "Final Score: " + score + "/3";
  finalResult.style.color = score === 3 ? "#28a745" : "#24292e";
}
</script>
