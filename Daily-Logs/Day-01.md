# Day 01 - Introduction to Node.js

**Date:** 2026-07-09

---

## 🎯 Goal

Understand what Node.js is, why it was created, and how it executes JavaScript outside the browser.

---

## 📚 Topics Covered

- What is a Runtime?
- What is Node.js?
- V8 Engine
- Node APIs
- JavaScript outside the browser
- Single Thread
- Asynchronous I/O
- Event Loop (High-level)

---

## 💡 Key Takeaways

- Node.js is a JavaScript runtime, not a programming language.
- A runtime is the environment responsible for executing JavaScript.
- Node.js combines the V8 engine with Node APIs and other internal components.
- JavaScript still runs on a single main thread.
- Long-running I/O operations are delegated instead of blocking the main thread.
- The Event Loop schedules callbacks after asynchronous operations complete.

---

## 🤔 Things That Confused Me

- How does the Event Loop know an operation has finished?
- What exactly is libuv?
- What's the difference between the Event Loop and libuv?

---

## 📝 Questions I Asked

1. What happens to the main thread while the database is responding?
2. How does the Event Loop know when an async task is finished?
3. Why does `setTimeout(..., 0)` execute after synchronous code?

---

## ✅ Mentor Feedback

- I understood the overall execution flow correctly.
- I need a deeper understanding of libuv.
- I should avoid saying "asynchronous code runs later"; instead:
  > Asynchronous operations start immediately, but their results become available later.

---

## 🚀 Tomorrow's Goal

Learn:

- V8
- libuv
- Event Loop
- Thread Pool
- Callback Queue