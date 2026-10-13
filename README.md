

# 🃏 Random Walk Card Game Simulator

Welcome to the **Random Walk Card Game Simulator**! This interactive educational tool demonstrates the mathematical concept of a 1-Dimensional Random Walk using a standard deck of playing cards.

👉 [Play the Simulator Here](https://aintoha.github.io/DrawCards/)

---

## 🎲 What is a Random Walk?
A random walk is a mathematical object that describes a path consisting of a succession of random steps. It is widely used in physics (Brownian motion), economics (stock market fluctuations), and computer science. 

In this 1D simulation, you start at position `0` on a number line and take steps left or right based on random chance.

## 📜 Game Rules
This simulator uses a deck of 52 playing cards (drawn with replacement) to determine the direction of each step:

*   🟥 **Red Cards (Hearts ♥ / Diamonds ♦):** Take **+1 step** forward (Right).
*   ⬛ **Black Cards (Spades ♠ / Clubs ♣):** Take **-1 step** backward (Left).

## ✨ Features
*   **Interactive Drawing:** Draw cards one by one to see your position change in real-time.
*   **Custom Trial Limits:** Set a "Maximum Draws" limit per experiment to see where you end up after $N$ steps.
*   **Horizontal Movement Log:** Tracks your exact sequence of draws, the direction taken, and your running position for each distinct trial.
*   **Combinatorics Calculator:** Dynamically calculates the total number of possible paths ($2^N$) based on your chosen number of maximum draws.

---

## 🧠 The Math Behind the Game (Combinatorics)

Every time you draw a card, there are exactly **2 possible outcomes** for your movement: Right (+1) or Left (-1). 

Because each draw is independent (the card is replaced and the deck is reshuffled), the total number of possible paths you can take grows exponentially. The formula for the total number of possible combinations is **$2^N$**, where **$N$** is the number of draws.

**Examples:**
*   **1 Draw:** $2^1 = 2$ possible paths.
*   **3 Draws:** $2^3 = 8$ possible paths.
*   **10 Draws:** $2^{10} = 1,024$ possible paths!

Despite thousands of possible paths, random walks tend to cluster around the starting point (0) over time, demonstrating the concept of "regression to the mean."

---

## 🚀 How to Run Locally
Since this simulator is built as a single, self-contained HTML file, running it is incredibly simple:
1. Clone or download this repository.
2. Double-click `index.html` to open it in any modern web browser (Chrome, Firefox, Safari, Edge).
3. No servers or dependencies required!
