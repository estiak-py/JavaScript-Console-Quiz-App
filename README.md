# JavaScript-Console-Quiz-App
Quiz game
# 🎯 JavaScript Console Quiz App

A simple beginner-friendly quiz application built using only JavaScript.  
This project runs in the browser console or Node.js and helps practice basic JavaScript logic.

---

## 🚀 Features
- Multiple questions quiz system
- User input using prompt()
- Score calculation system
- Instant correct/incorrect feedback
- Fully built with vanilla JavaScript (No HTML/CSS required)

---

## 🧠 Concepts Used
- Arrays & Objects
- Loops (for loop)
- Conditionals (if/else)
- Functions
- Console input/output

---

## 📜 How It Works
1. User is asked questions one by one
2. User types answers
3. System checks answers
4. Final score is displayed

---

## 💻 Code Example

```javascript
const questions = [
  { question: "2 + 2 কত?", answer: "4" },
  { question: "JavaScript কে বানিয়েছে?", answer: "Brendan Eich" },
  { question: "HTML এর full form কি?", answer: "HyperText Markup Language" }
];

let score = 0;

for (let i = 0; i < questions.length; i++) {
  let userAnswer = prompt(questions[i].question);

  if (userAnswer === questions[i].answer) {
    console.log("✔ Correct!");
    score++;
  } else {
    console.log("❌ Wrong!");
  }
}

console.log("🎯 Final Score: " + score + "/" + questions.length);
