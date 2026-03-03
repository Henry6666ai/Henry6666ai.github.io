---
layout: default
title: Chapter 24 - Inflation
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# 💸 Module: Measuring the Cost of Living

To understand how "expensive" life is getting, economists use the **Consumer Price Index (CPI)**. It’s essentially a snapshot of the average cost of survival for a typical consumer.

---

## 📊 The Consumer Price Index (CPI)
The CPI is a measure of the overall level of prices for goods and services bought by a typical consumer. It is computed and reported every month by the **Bureau of Labor Statistics (BLS)**.

### How to Calculate CPI in 5 Steps
1. **Fix the Basket:** Determine which prices are most important to the typical consumer.
2. **Find the Prices:** Identify the prices of those goods at each point in time.
3. **Compute the Basket's Cost:** Use the same basket of goods to isolate price changes.
4. **Choose a Base Year:** Use the following formula:
   $$\text{CPI} = \left( \frac{\text{Price of basket in current year}}{\text{Price of basket in base year}} \right) \times 100$$
5. **Compute the Inflation Rate:** Calculate the percentage change from the preceding period.

---

## ⚠️ Problems with the CPI
The CPI isn't perfect and often **overstates** the true cost of living due to:

* **Substitution Bias:** Consumers switch to cheaper goods when prices rise, but the "fixed basket" doesn't account for this.
* **Introduction of New Goods:** More variety makes each dollar more valuable.
* **Unmeasured Quality Change:** If a product gets better but the price stays the same, your "real" cost actually dropped.

---

## ⚔️ GDP Deflator vs. CPI

| Feature | GDP Deflator | Consumer Price Index (CPI) |
| :--- | :--- | :--- |
| **Focus** | Prices of all goods & services produced domestically. | Prices of goods & services bought by consumers. |
| **Imported Goods** | **Excluded** (not produced here). | **Included** (if consumers buy them). |
| **Basket Type** | Currently produced goods. | Fixed basket of goods. |

---

## 🌡️ Real vs. Nominal Interest Rates
To understand the true return on a loan or investment, we must correct for inflation.

* **Nominal Interest Rate:** The rate as usually reported (without inflation correction).
* **Real Interest Rate:** The rate corrected for the effects of inflation.

$$\text{Real Interest Rate} = \text{Nominal Interest Rate} - \text{Inflation Rate}$$

> **Pro Tip:** In periods of deflation (falling prices), the real interest rate actually exceeds the nominal interest rate.

---

## 📝 Practice Quiz

<div id="quiz-container" style="background-color: #f8f9fa; padding: 25px; border-radius: 10px; border: 1px solid #d1d5da; color: #24292e; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;">
  
  <div id="q1-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>1. Who is responsible for computing and reporting the CPI every month?</strong></p>
    <label style="display: block;"><input type="radio" name="q1" value="wrong"> The Federal Reserve</label>
    <label style="display: block;"><input type="radio" name="q1" value="correct"> The Bureau of Labor Statistics (BLS)</label>
    <label style="display: block;"><input type="radio" name="q1" value="wrong"> The Internal Revenue Service (IRS)</label>
    <div id="feedback-q1" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q2-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>2. If the price of an imported French wine increases, which index is affected?</strong></p>
    <label style="display: block;"><input type="radio" name="q2" value="wrong"> The GDP Deflator</label>
    <label style="display: block;"><input type="radio" name="q2" value="correct"> The CPI</label>
    <label style="display: block;"><input type="radio" name="q2" value="wrong"> Both the GDP Deflator and the CPI</label>
    <div id="feedback-q2" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q3-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>3. If your bank gives you a 5% nominal interest rate and inflation is 2%, what is your real interest rate?</strong></p>
    <label style="display: block;"><input type="radio" name="q3" value="wrong"> 7%</label>
    <label style="display: block;"><input type="radio" name="q3" value="wrong"> 2.5%</label>
    <label style="display: block;"><input type="radio" name="q3" value="correct"> 3%</label>
    <div id="feedback-q3" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div style="text-align: center;">
    <button onclick="checkQuiz24()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-weight: bold;">Check Answers</button>
    <h3 id="score-display" style="margin-top: 20px;"></h3>
  </div>
</div>

<script>
function checkQuiz24() {
  let score = 0;
  const total = 3;
  const results = {
    q1: { correct: "correct", msg: "Correct! The BLS handles the monthly reporting of the CPI." },
    q2: { correct: "correct", msg: "Correct! The CPI includes imports bought by consumers; the GDP Deflator only reflects domestic production." },
    q3: { correct: "correct", msg: "Correct! 5% - 2% = 3%." }
  };
  const errors = {
    q1: "Incorrect. The correct answer is the Bureau of Labor Statistics (BLS).",
    q2: "Incorrect. Since the wine is imported, it is only in the CPI, not the GDP Deflator.",
    q3: "Incorrect. Real Rate = Nominal - Inflation (5 - 2 = 3)."
  };

  for (let i = 1; i <= total; i++) {
    const qName = 'q' + i;
    const selected = document.querySelector(`input[name="${qName}"]:checked`);
    const feedback = document.getElementById(`feedback-${qName}`);
    const box = document.getElementById(`${qName}-box`);

    if (selected) {
      if (selected.value === "correct") {
        score++;
        feedback.innerHTML = "✅ " + results[qName].msg;
        feedback.style.color = "#28a745";
        box.style.backgroundColor = "#e6ffed";
      } else {
        feedback.innerHTML = "❌ " + errors[qName];
        feedback.style.color = "#d73a49";
        box.style.backgroundColor = "#ffeef0";
      }
    }
  }
  document.getElementById('score-display').innerHTML = "Your Score: " + score + " / " + total;
}
</script>

---
[⬅ Back to Chapter 23 (GDP)](index.html)
