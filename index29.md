---
layout: default
title: Chapter 29 - The Monetary System
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# 💸 Chapter 29: The Monetary System

Money is the set of assets in an economy that people regularly use to buy goods and services from others. It eliminates the need for a **"double coincidence of wants"** required in a barter system.

---

## 1. The Three Functions of Money

* **Medium of Exchange:** An item that buyers give to sellers when they want to purchase goods and services.
* **Unit of Account:** The yardstick people use to post prices and record debts.
* **Store of Value:** An item that people can use to transfer purchasing power from the present to the future.

### Types of Money
1.  **Commodity Money:** Money that takes the form of a commodity with intrinsic value (e.g., gold, cigarettes in POW camps).
2.  **Fiat Money:** Money without intrinsic value that is used as money because of government decree (e.g., the U.S. dollar).

---

## 2. Measuring the Money Stock

The money stock is the quantity of money circulating in the economy. It is divided into two main categories:

| Measure | Components |
| :--- | :--- |
| **M1** | Currency, demand deposits, traveler’s checks, and other checkable deposits. |
| **M2** | Everything in M1 plus savings deposits, small time deposits, and money market mutual funds. |

> **Note:** As of 2019, there was approximately **$1.7 trillion** in currency outstanding. Much of this is held abroad or used in the informal economy.

---

## 3. The Federal Reserve System

The **Federal Reserve (the Fed)** is the central bank of the United States, established in 1913.

### Organization
* **Board of Governors:** 7 members appointed by the president for 14-year terms. 
* **Regional Banks:** 12 Federal Reserve Banks located across major U.S. cities.
* **Federal Open Market Committee (FOMC):** The policy-making body consisting of the 7 governors and 5 regional bank presidents. They meet every 6 weeks to discuss monetary policy.

---

## 4. Banks and the Money Supply

Banks operate under a **fractional-reserve banking** system, where they keep only a fraction of deposits as reserves and lend out the rest.

* **Reserve Ratio ($R$):** The fraction of total deposits that a bank holds as reserves.
* **The Money Multiplier:** The amount of money the banking system generates with each dollar of reserves.

$$\text{Money Multiplier} = \frac{1}{R}$$

REFER TO FIGURE 1: THE MONEY MULTIPLIER PROCESS

---

## 5. Tools of Monetary Control

The Fed influences the quantity of money in the economy using four primary tools:

1.  **Open-Market Operations:** The buying and selling of U.S. government bonds. 
    * *Buying bonds* increases the money supply.
    * *Selling bonds* decreases the money supply.
2.  **Fed Lending:** Changing the **Discount Rate** (the interest rate on loans the Fed makes to banks).
3.  **Reserve Requirements:** Regulations on the minimum amount of reserves that banks must hold against deposits.
4.  **Interest on Reserves:** When the Fed pays a higher interest rate on reserves, banks choose to hold more reserves, which decreases the money supply.

---

## 6. The Federal Funds Rate

The federal funds rate is the short-term interest rate that banks charge one another for overnight loans. 

* **To decrease the rate:** The Fed buys bonds, injecting reserves into the banking system.
* **To increase the rate:** The Fed sells bonds, removing reserves from the banking system.

---

## 📝 Practice Quiz

<div id="quiz-container" style="background-color: #f8f9fa; padding: 25px; border-radius: 10px; border: 1px solid #d1d5da; color: #24292e; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;">

  <div id="q1-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>1. Which function of money is being used when you check the price of a laptop to see if you can afford it?</strong></p>
    <label style="display: block;"><input type="radio" name="q1" value="A"> A) Medium of exchange</label>
    <label style="display: block;"><input type="radio" name="q1" value="B"> B) Unit of account</label>
    <label style="display: block;"><input type="radio" name="q1" value="C"> C) Store of value</label>
    <div id="feedback-q1" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q2-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>2. If the reserve ratio is 10%, what is the money multiplier?</strong></p>
    <label style="display: block;"><input type="radio" name="q2" value="A"> A) 1</label>
    <label style="display: block;"><input type="radio" name="q2" value="B"> B) 5</label>
    <label style="display: block;"><input type="radio" name="q2" value="C"> C) 10</label>
    <label style="display: block;"><input type="radio" name="q2" value="D"> D) 20</label>
    <div id="feedback-q2" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q3-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>3. What is the Fed’s primary tool for changing the money supply?</strong></p>
    <label style="display: block;"><input type="radio" name="q3" value="A"> A) Changing reserve requirements</label>
    <label style="display: block;"><input type="radio" name="q3" value="B"> B) Adjusting the discount rate</label>
    <label style="display: block;"><input type="radio" name="q3" value="C"> C) Open-market operations</label>
    <div id="feedback-q3" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div id="q4-box" style="margin-bottom: 20px; padding: 15px; border-radius: 8px;">
    <p><strong>4. Fiat money is defined as money that:</strong></p>
    <label style="display: block;"><input type="radio" name="q4" value="A"> A) Has intrinsic value</label>
    <label style="display: block;"><input type="radio" name="q4" value="B"> B) Is backed by gold</label>
    <label style="display: block;"><input type="radio" name="q4" value="C"> C) Is used because of government decree</label>
    <div id="feedback-q4" style="margin-top: 10px; font-weight: 600;"></div>
  </div>

  <div style="text-align: center;">
    <button onclick="checkQuiz29()" style="background-color: #2ea44f; color: white; border: none; padding: 12px 25px; border-radius: 6px; cursor: pointer; font-weight: bold;">Submit Answers</button>
    <h3 id="score-display" style="margin-top: 20px;"></h3>
  </div>
</div>

<script>
function checkQuiz29() {
  let score = 0;
  const total = 4;
  const solutions = {
    q1: { ans: "B", note: "A unit of account is the yardstick used to post prices and measure value." },
    q2: { ans: "C", note: "The formula is 1/R. So 1 / 0.10 = 10." },
    q3: { ans: "C", note: "Open-market operations are the Fed's most frequently used tool." },
    q4: { ans: "C", note: "Fiat money has no intrinsic value and is established by government decree." }
  };

  for (let i = 1; i <= total; i++) {
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
        feedback.innerHTML = "❌ Wrong. The correct answer is " + solutions[qName].ans + ". " + solutions[qName].note;
        feedback.style.color = "#d73a49";
        box.style.backgroundColor = "#ffeef0";
      }
    }
  }
  document.getElementById('score-display').innerHTML = "Final Score: " + score + " / " + total;
}
</script>

---
[⬅ Back to Chapter 26](index26.html) | [🏠 Home](index.html)
