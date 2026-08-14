# Bullet Line: Scripture Pursuit (KJV)

**Bullet Line: Scripture Pursuit** is an engaging, high-speed King James Version (KJV) Bible trivia game built as a self-contained web application. Test your knowledge of the Old and New Testaments, build your silver treasury, and outrun the incoming derailment!

---

## 🚀 Core Features

* **KJV Scripture Integration:** Every trivia question is paired with a direct King James Bible reference and scripture quote to deepen your study and understanding of the Word.
* **The Cash Builder Round:** A fast-paced 60-second opening round where you bank 1,000 Shekels of Silver for every correct answer.
* **Dynamic Chase Mechanics:** Navigate the 7-step train board as you try to outrun an approaching Derailment. Correct answers move your Bullet Train toward the station while incorrect answers let the chaser close the gap.
* **Procedural Web Audio API Sound Effects:** Fully self-contained sound effects and train ambient audio generated programmatically via JavaScript—no external audio assets required.
* **Responsive & Immersive UI:** Features a custom neon train CSS layout, animated fog background, mobile-optimized scripture viewing drawers, and dynamic game statistics tracking.

---

## 🎮 How to Play

1. **Start the Game:** Click the **START GAME** button on the main screen.
2. **The Builder Round:** Answer as many KJV Bible questions as you can within 60 seconds to stack up your starting Shekels of Silver.
3. **Choose Your Head Start:** Select your track position based on your accumulated bank (Lower Track, Current Bank, or Express Line).
4. **The Chase:** Answer difficulty-scaled questions (Easy, Medium, Hard) to advance your Bullet Train to the station (Step 0) while keeping ahead of the Derailment!

---

## 📊 Game Summary Report

After each game concludes (win or loss), a detailed **Game Summary Report** is displayed showing:

* **Question-by-Question Breakdown:** Every question you answered during the game, listed in order with:
  * Your choice vs. the correct answer
  * Result badge (✓ CORRECT or ✗ INCORRECT)
  * The KJV scripture reference paired with each question
  * The full scripture text for deeper study
* **Game Statistics:** A running total at the bottom tracks:
  * Total games played
  * Games won
  * Games lost
* **Share & Restart Options:** Copy your results or start a fresh game immediately.

This report helps reinforce biblical knowledge and track your progress over multiple play sessions.

---

## 🔄 Question Deck Shuffle Logic

The game uses a **smart deck shuffling system** to ensure a fresh experience while preventing question fatigue:

* **Session Persistence:** Used question IDs are tracked in browser localStorage (`bulletline_used_questions`), preventing the same question from appearing twice in a single session.
* **Automatic Reshuffling:** When all questions in the master deck have been asked, a shuffle modal appears notifying you that the deck is being reset. The used question log is cleared, and all 400+ questions become available again.
* **Graceful Fallback:** If localStorage is unavailable (e.g., private browsing mode or embedded browsers), the question deck still tracks usage in-memory for that session only—you won't replay questions until you reload the page.
* **Randomized Draw:** Active questions are randomly shuffled on each reset to ensure varied game experiences.

---

## 📂 Project Structure

This project is engineered for single-file portability, meaning all HTML structure, CSS styling, SVG graphics, audio synthesis logic, and the complete 400+ question bank live directly inside a single file:
* `index.html` — The complete application source.

---

## 📜 License

This work is protected and licensed under the **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0)**. 

© 2026 William Monti. See the [LICENSE](LICENSE) file for more details.
