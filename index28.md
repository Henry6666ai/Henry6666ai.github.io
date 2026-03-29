---
layout: default
title: Chapter 28 - Unemployment
---

# 📉 Chapter 28: Unemployment

This chapter explores how economists measure the "unemployment rate," the problems with these measurements, and why there are always some people without jobs even in a healthy economy.

---

## 🔍 1. Identifying Unemployment
The Bureau of Labor Statistics (BLS) divides the adult population (ages 16 and older) into three distinct categories:

* **Employed:** Those who worked as paid employees, worked in their own business, or worked as unpaid workers in a family member’s business. Includes both full-time and part-time workers.
* **Unemployed:** Those who were not employed but were available for work and had tried to find employment during the previous **four weeks**.
* **Not in the Labor Force:** Those who fit neither category, such as full-time students, homemakers, and retirees.

<div style="text-align: center; margin: 25px 0;">
  <img src="population-breakdown.png" alt="Figure 1 - The Breakdown of the Population" loading="lazy" style="max-width: 90%; border-radius: 8px; border: 1px solid #ddd; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
  <p style="color: #6a737d; font-style: italic; font-size: 0.9em; margin-top: 10px;">
    Figure 1: The Breakdown of the Population. Shows the relative sizes of the employed, unemployed, and those not in the labor force.
  </p>
</div>

---

## 🧮 2. Measuring the Labor Market
We use two primary statistics to gauge the health of the labor market:

**Labor Force**
The total number of workers, including both the employed and the unemployed.
$$\text{Labor Force} = \text{Number of Employed} + \text{Number of Unemployed}$$

**Unemployment Rate**
The percentage of the labor force that is unemployed.
$$\text{Unemployment Rate} = \frac{\text{Number of Unemployed}}{\text{Labor Force}} \times 100$$

**Labor-Force Participation Rate**
The percentage of the total adult population that is in the labor force.
$$\text{Participation Rate} = \frac{\text{Labor Force}}{\text{Adult Population}} \times 100$$

---

## 📈 3. Trends and Real-World Data
Labor-market experiences differ significantly across demographic groups. Over the last several decades, the labor-force participation rate for women has risen dramatically, while the rate for men has gradually declined.

<div style="text-align: center; margin: 25px 0;">
  <img src="labor-force-participation.png" alt="Figure 2 - Labor-Force Participation Rates" loading="lazy" style="max-width: 90%; border-radius: 8px; border: 1px solid #ddd;">
  <p style="color: #6a737d; font-style: italic; font-size: 0.9em; margin-top: 10px;">
    Figure 2: Converging participation rates of men and women since 1950.
  </p>
</div>

---

## ⏳ 4. Why is there Always Unemployment?
The **Natural Rate of Unemployment** persists even in the long run.

* **Frictional Unemployment:** Time spent searching for the right job match.
* **Structural Unemployment:** A fundamental mismatch between the number of jobs and seekers, often due to wages being stuck above equilibrium.
* **Cyclical Unemployment:** Short-term fluctuations tied to the business cycle.

---

## ⚖️ 5. Causes of Structural Unemployment
Structural unemployment happens when the wage is stuck above the equilibrium level.

1. **Minimum-Wage Laws:** Creates a labor surplus if set above equilibrium.
2. **Unions:** Collective bargaining can push wages up for "insiders."
3. **Efficiency Wages:** Firms pay more to boost productivity (Health, Turnover, Quality, Effort).

<div style="text-align: center; margin: 25px 0;">
  <img src="unemployment-from-a-wage-above-equilibrium.png" alt="Figure 3 - Wage Above Equilibrium" loading="lazy" style="max-width: 90%; border-radius: 8px; border: 1px solid #ddd;">
  <p style="color: #6a737d; font-style: italic; font-size: 0.9em; margin-top: 10px;">
    Figure 3: A wage floor creates a labor surplus (unemployment).
  </p>
</div>

---

## 📝 Practice Quiz

<div id="quiz-container" style="background-color: #f8f9fa; padding: 25px; border-radius: 10px; border: 1px solid #d1d5da; color: #24292e; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;">

  <div id="q1-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>1. A person who is not working and has not looked for work in the last six weeks is classified as:</strong></p>
    <label style="display: block;"><input type="radio" name="q1" value="A"> A) Employed</label>
    <label style="display: block;"><input type="radio" name="q1" value="B"> B) Unemployed</label>
    <label style="display: block;"><input type="radio" name="q1" value="C"> C) Not in the labor force</label>
    <div id="feedback-q1" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q2-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>2. Which of the following would decrease the unemployment rate?</strong></p>
    <label style="display: block;"><input type="radio" name="q2" value="A"> A) An increase in minimum wage</label>
    <label style="display: block;"><input type="radio" name="q2" value="B"> B) A more efficient job-search website</label>
    <label style="display: block;"><input type="radio" name="q2" value="C"> C) People quitting to go back to school</label>
    <div id="feedback-q2" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div style="text-align: center;">
    <button onclick="checkQuiz28()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-weight: bold;">Check Answers</button>
    <h3 id="score-display" style="margin-top: 20px;"></h3>
  </div>
</div>

---
[⬅ Back to Chapter 26](index26.html) | [🏠 Home](index.html)

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

<script>
function checkQuiz28() {
  let score = 0;
  const solutions = {
    q1: { ans: "C", txt: "To be 'unemployed,' a person must have actively looked for work within the previous 4 weeks." },
    q2: { ans: "B", txt: "Efficient job-search tools reduce frictional unemployment." }
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
        feedback.innerHTML = "❌ Wrong. Correct: " + solutions[qName].ans + ". " + solutions[qName].txt;
        feedback.style.color = "#d73a49";
        box.style.backgroundColor = "#ffeef0";
      }
    }
  }
  document.getElementById('score-display').innerHTML = "Score: " + score + " / 2";
}
</script>
