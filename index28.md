---
layout: default
title: Chapter 28 - Unemployment
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$', '$$'], ['\\[', '\\]']],
      processEscapes: true
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# 📉 Chapter 28: Unemployment

This chapter explores how economists measure the **unemployment rate**, the problems with these measurements, and why there are always some people without jobs even in a healthy economy.

---

## 🔍 1. Identifying Unemployment
The Bureau of Labor Statistics (BLS) divides the adult population (16+) into three categories:

* **Employed:** Paid employees, self-employed, or unpaid workers in a family business.
* **Unemployed:** Not employed, but available for work and have **actively looked** for work in the last 4 weeks.
* **Not in the Labor Force:** Full-time students, homemakers, and retirees.

<div style="text-align: center; margin: 30px 0;">
  <img src="population-breakdown.png" alt="Figure 1 - Population Breakdown" style="max-width: 90%; border: 1px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <p style="color: #6a737d; font-style: italic; font-size: 0.9em; margin-top: 10px;">Figure 1: The Breakdown of the Population</p>
</div>

---

## 🧮 2. Measuring the Labor Market
These formulas are formatted using block LaTeX for maximum clarity:

**Labor Force**
$$\text{Labor Force} = \text{Number of Employed} + \text{Number of Unemployed}$$

**Unemployment Rate**
$$\text{Unemployment Rate} = \left( \frac{\text{Number of Unemployed}}{\text{Labor Force}} \right) \times 100$$

**Labor-Force Participation Rate**
$$\text{Participation Rate} = \left( \frac{\text{Labor Force}}{\text{Adult Population}} \right) \times 100$$

---

## 📈 3. Trends and Real-World Data
Labor-market experiences differ across groups. Since 1950, women's participation has surged while men's has gradually declined.

<div style="text-align: center; margin: 30px 0;">
  <img src="labor-force-participation.png" alt="Figure 2 - Participation Trends" style="max-width: 90%; border: 1px solid #ddd; border-radius: 8px;">
  <p style="color: #6a737d; font-style: italic; font-size: 0.9em; margin-top: 10px;">Figure 2: Labor-Force Participation Rates for Men and Women</p>
</div>

---

## ⏳ 4. Why is there Always Unemployment?
The **Natural Rate of Unemployment** is the "normal" level of unemployment that doesn't go away on its own.

* **Frictional Unemployment:** The time it takes for workers to find jobs that best suit their skills (**Job Search**).
* **Structural Unemployment:** When the number of jobs is insufficient for the number of seekers (usually because wages are stuck too high).
* **Cyclical Unemployment:** Short-term fluctuations around the natural rate caused by the business cycle.

---

## ⚖️ 5. Causes of Structural Unemployment
Structural unemployment happens when the wage is stuck above the equilibrium level ($W > W_{eq}$).

1.  **Minimum-Wage Laws:** Creates a labor surplus if set above equilibrium.
2.  **Unions:** Collective bargaining can push wages up, benefiting "insiders" but leaving "outsiders" unemployed.
3.  **Efficiency Wages:** Firms pay more to increase productivity (better health, lower turnover, higher quality).

<div style="text-align: center; margin: 30px 0;">
  <img src="unemployment-from-a-wage-above-equilibrium.png" alt="Figure 3 - Wage Above Equilibrium" style="max-width: 90%; border: 1px solid #ddd; border-radius: 8px;">
  <p style="color: #6a737d; font-style: italic; font-size: 0.9em; margin-top: 10px;">Figure 3: Unemployment resulting from a wage floor above equilibrium.</p>
</div>

---

## 📝 Practice Quiz

<div id="quiz-container" style="background-color: #f8f9fa; padding: 25px; border-radius: 10px; border: 1px solid #d1d5da; color: #24292e;">

  <div class="q-box" style="margin-bottom: 25px;">
    <p><strong>1. A person who is not working and has not looked for work in the last six weeks is:</strong></p>
    <label style="display: block;"><input type="radio" name="q1" value="A"> A) Employed</label>
    <label style="display: block;"><input type="radio" name="q1" value="B"> B) Unemployed</label>
    <label style="display: block;"><input type="radio" name="q1" value="C"> C) Not in the labor force</label>
    <div id="feedback-q1" style="margin-top: 10px; font-weight: bold;"></div>
  </div>

  <div class="q-box" style="margin-bottom: 25px;">
    <p><strong>2. Which of the following would decrease the unemployment rate?</strong></p>
    <label style="display: block;"><input type="radio" name="q2" value="A"> A) An increase in minimum wage</label>
    <label style="display: block;"><input type="radio" name="q2" value="B"> B) A more efficient job-search website</label>
    <div id="feedback-q2" style="margin-top: 10px; font-weight: bold;"></div>
  </div>

  <div class="q-box" style="margin-bottom: 25px;">
    <p><strong>3. "Efficiency Wages" are paid to:</strong></p>
    <label style="display: block;"><input type="radio" name="q3" value="A"> A) Increase profitability through higher productivity</label>
    <label style="display: block;"><input type="radio" name="q3" value="B"> B) Comply with government regulations</label>
    <div id="feedback-q3" style="margin-top: 10px; font-weight: bold;"></div>
  </div>

  <div class="q-box" style="margin-bottom: 25px;">
    <p><strong>4. Structural unemployment is associated with:</strong></p>
    <label style="display: block;"><input type="radio" name="q4" value="A"> A) Wages being held above the equilibrium level</label>
    <label style="display: block;"><input type="radio" name="q4" value="B"> B) A graduate finding their first job</label>
    <div id="feedback-q4" style="margin-top: 10px; font-weight: bold;"></div>
  </div>

  <div class="q-box" style="margin-bottom: 25px;">
    <p><strong>5. What is the difference between frictional and structural?</strong></p>
    <label style="display: block;"><input type="radio" name="q5" value="A"> A) Frictional is long-term; structural is short-term</label>
    <label style="display: block;"><input type="radio" name="q5" value="B"> B) Frictional involves searching; structural involves a lack of jobs</label>
    <div id="feedback-q5" style="margin-top: 10px; font-weight: bold;"></div>
  </div>

  <button onclick="checkQuiz()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-weight: bold;">Check Answers</button>
  <h3 id="score" style="margin-top: 20px;"></h3>
</div>

<script>
function checkQuiz() {
  let score = 0;
  const sol = {
    q1: { a: "C", e: "To be 'unemployed,' a person must have searched for work within the previous four weeks." },
    q2: { a: "B", e: "Increasing the efficiency of job matching reduces frictional unemployment." },
    q3: { a: "A", e: "Firms pay higher wages to improve worker health, turnover, and effort." },
    q4: { a: "A", e: "Structural surplus happens when wages are stuck above equilibrium." },
    q5: { a: "B", e: "Frictional is about the matching process; structural is about a fundamental job shortage at the current wage." }
  };

  for (let i = 1; i <= 5; i++) {
    const q = 'q' + i;
    const sel = document.querySelector(`input[name="${q}"]:checked`);
    const f = document.getElementById('feedback-' + q);
    if (sel) {
      if (sel.value === sol[q].a) {
        score++;
        f.innerHTML = "✅ Correct!";
        f.style.color = "green";
      } else {
        f.innerHTML = "❌ Wrong. Correct answer is " + sol[q].a + ". " + sol[q].e;
        f.style.color = "red";
      }
    }
  }
  document.getElementById('score').innerHTML = "Final Score: " + score + " / 5";
}
</script>
