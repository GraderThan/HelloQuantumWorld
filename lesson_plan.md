# Lesson Plan: Introduction to Quantum Computing

---

## Overview

| | |
|---|---|
| **Grade Level** | Middle School and High School (Grades 6-12) |
| **Duration** | 90 minutes |
| **Prerequisites** | Basic understanding of computers and binary (0s and 1s) |

---

## Learning Objectives

By the end of this lesson, students will be able to:

1. **Explain** the difference between classical bits and quantum bits (qubits)
2. **Describe** superposition using the "spinning coin" analogy
3. **Describe** entanglement using the "magic gloves" analogy
4. **Experience** running code on a real quantum computer
5. **Discuss** why quantum computing matters for the future

---

## Materials Needed

### For the Teacher
- Computer with internet access and projector
- Grader Than Workspace with the Hello Quantum World notebook
- IBM Quantum account with API token ([sign up free](https://quantum.ibm.com/))
- A large coin for demonstration
- Whiteboard and markers

### For Students
- Grader Than Workspace (one per student or group)
- Coins (one per student) for the superposition activity
- Two paper clips per student for the entanglement activity
- Cheat sheet printout (optional but helpful)

---

## Lesson Outline

### 1. Introduction (10 minutes)

#### Hook: The Spinning Coin

Start with a simple question:

> **"If I flip this coin, what are the possible outcomes?"**

Students will answer: Heads or Tails.

Now spin the coin on a table and ask:

> **"While the coin is spinning, is it heads or tails?"**

Let students discuss. The answer: It's *both* — until it stops and we look at it.

#### Set the Stage

Explain that today they'll learn about quantum computers, which work in a way that's similar to that spinning coin. And the best part? They'll actually run code on a real quantum computer!

#### Teacher Tips
- Keep the energy high — this is exciting stuff!
- Emphasize that quantum computers aren't just "faster computers" — they work in a fundamentally different way
- It's okay to say "scientists are still figuring this out" — quantum physics is genuinely strange

---

### 2. Classical Computing Review (5 minutes)

#### Quick Review: Bits

Ask students what they know about how computers store information.

Key points to cover:
- Computers use **bits** — the smallest unit of information
- A bit can only be **0** or **1** (like a light switch: off or on)
- Everything a computer does — games, videos, apps — comes down to billions of 0s and 1s

#### Analogy
> A bit is like a coin lying flat on a table. It's either heads (1) or tails (0). Never both.

---

### 3. Quantum Basics — Direct Instruction (15 minutes)

#### Introducing Qubits

Explain that quantum computers use **qubits** instead of bits.

> **"A qubit is like that spinning coin. While it's spinning, it's both 0 AND 1 at the same time. This is called superposition."**

#### Superposition

**Definition:** A qubit can be 0, 1, or *both at the same time* until we measure it.

**Demonstration:** Spin your coin again. While spinning, it represents superposition. When it lands, it "collapses" to one value — just like measuring a qubit.

**Why it matters:** This allows quantum computers to explore many possibilities simultaneously, making them powerful for certain types of problems.

#### Entanglement

**Definition:** When two qubits become "linked" so that measuring one instantly tells you about the other — no matter how far apart they are.

**Analogy — The Magic Gloves:**
> Imagine you have a pair of gloves in two boxes. You send one box to your friend on the other side of the world. When you open your box and see a left-hand glove, you *instantly* know your friend has the right-hand glove — even before they open their box.
>
> With quantum entanglement, it's even stranger: the gloves don't "decide" which is left and which is right until someone opens a box!

Einstein called this "spooky action at a distance" because it seemed so weird.

#### Measurement

**Key concept:** When we measure a qubit, we force it to "choose" — it stops being both 0 and 1 and becomes just one.

This is why quantum computing is tricky: we have to be clever about when and how we measure.

#### Teacher's Quick Reference

| Concept | Classical | Quantum |
|---------|-----------|---------|
| Basic unit | Bit | Qubit |
| Possible states | 0 OR 1 | 0 AND 1 (until measured) |
| Analogy | Coin lying flat | Coin spinning |

---

### 4. Hands-On Activity: Superposition with Coins (10 minutes)

#### Setup
Give each student a coin.

#### Activity

**Part 1 — Classical Bit:**
- Have students flip their coin and let it land
- Record: Heads = 1, Tails = 0
- Discuss: This is how a classical bit works — it's one or the other

**Part 2 — Qubit in Superposition:**
- Have students spin their coin on the desk
- While spinning, ask: "Is it heads or tails?"
- Answer: It's both! This represents superposition

#### Discussion Questions
- "What happens when the coin stops spinning?" (It collapses to one state)
- "How is this like measuring a qubit?" (Measurement forces it to choose)

---

### 5. Interactive Game: Quantum Tic-Tac-Toe (20 minutes)

#### Introduction

Introduce the Quantum Tic-Tac-Toe game, which lets students experience superposition and entanglement in a familiar game.

**Game Link:** [https://quantumtictactoe.com/play](https://quantumtictactoe.com/play)

Alternative link: [https://everthemore.itch.io/tiqtaqtoe](https://everthemore.itch.io/tiqtaqtoe)

#### Setup
- Divide students into pairs
- Each pair accesses the game on a computer or tablet
- Start with "Minimal Quantum" setting, then increase quantumness

#### How It Works
- **Superposition moves:** Place your X or O in *two* squares at once — it's in both until something forces it to collapse
- **Entanglement:** Moves can become linked to other moves
- **Measurement:** When the board gets complicated, moves collapse to definite positions

#### Gameplay (15 minutes)
Let students play several rounds, experimenting with different quantumness levels.

#### Discussion (5 minutes)
Bring the class together and ask:
- "How was this different from regular Tic-Tac-Toe?"
- "What strategies did you discover?"
- "How did entanglement affect your game?"

---

### 6. Hands-On Activity: Entanglement with Paper Clips (10 minutes)

#### Setup
Give each student two paper clips.

#### Activity

1. **Link your paper clips** into a chain of two
2. **Pair up** with a partner and connect your chains into a loop of four clips
3. **Without talking**, each person gently twists or moves one of their clips
4. **Observe** how movement in one part affects the whole structure

#### Discussion
> "Just like our paper clip loop, entangled qubits are connected. When something happens to one, it affects the other — instantly, no matter how far apart they are."

**Common question:** "Can we use entanglement to send messages instantly?"

**Answer:** Great question! Unfortunately, no. While the particles affect each other instantly, we can't control *what* message is sent. It's random — so no faster-than-light texting! Scientists are still working out exactly why this is.

---

### 7. Run Code on a Real Quantum Computer (15 minutes)

This is the highlight of the lesson!

#### Setup
- Open the `quantum_notebook.ipynb` in Grader Than Workspace
- Make sure your IBM Quantum API token is ready

#### Walk Through the Notebook
Guide students through each cell:

1. **Install tools** — Set up the software
2. **Connect to IBM Quantum** — Link to real quantum computers
3. **Create the circuit** — Build our quantum program (H gate + CX gate = entanglement!)
4. **Set up measurements** — Define what we want to observe
5. **Optimize** — Adapt our circuit for the specific quantum computer
6. **Run it!** — Send to the quantum computer and wait
7. **See results** — Verify that we created entanglement

#### While Waiting
The quantum computer queue may take a few minutes. Use this time to:
- Review the cheat sheet
- Discuss what's happening (your code is running on a real quantum computer!)
- Answer questions
- Complete the worksheet (if using one)

#### Celebrate the Results
When results come back, point out:
- **ZZ and XX values close to 1** = We created entanglement!
- Your students just ran code on one of the most advanced machines ever built

---

### 8. Real-World Applications (5 minutes)

Briefly discuss how quantum computers might change the world:

| Field | Quantum Application |
|-------|---------------------|
| **Medicine** | Simulating molecules to discover new drugs |
| **Security** | Breaking (and creating) new types of encryption |
| **Finance** | Optimizing investment strategies |
| **Climate** | Modeling complex climate systems |
| **AI** | Training machine learning models faster |

**Key message:** Quantum computers won't replace your laptop for everyday tasks, but they'll solve problems that regular computers *never* could — even with billions of years to work on them.

---

### 9. Wrap-Up and Reflection (5 minutes)

#### Quick Quiz (Oral)
1. "What's the difference between a bit and a qubit?"
2. "What is superposition?"
3. "What is entanglement?"
4. "What did we prove by running our quantum circuit?"

#### Reflection
Ask students to share:
- One thing they found surprising
- One question they still have

#### Closing
> "Today you ran code on a real quantum computer — something that wasn't possible for *anyone* just 10 years ago. Quantum computing is still in its early days, which means the biggest discoveries haven't been made yet. Maybe one of you will make them!"

---

## Differentiation Strategies

| Student Type | Approach |
|--------------|----------|
| **Visual learners** | Use diagrams, the circuit visualization, and the Bloch sphere (if going deeper) |
| **Kinesthetic learners** | Emphasize the coin spinning, paper clip, and game activities |
| **Advanced students** | Discuss quantum gates in more detail, explore IBM Quantum Composer |
| **Students needing support** | Pair with peers, focus on analogies over math, use the cheat sheet |

---

## Assessment Ideas

### Formative (During Lesson)
- Observe participation in activities
- Listen to discussions and questions
- Check understanding during the notebook walkthrough

### Summative (After Lesson)
- Short worksheet with multiple choice and short answer
- Exit ticket: "Explain superposition to someone who's never heard of it"
- Optional project: Research one application of quantum computing

---

## Common Student Questions (and Answers)

**Q: Will quantum computers replace regular computers?**
> A: Not for everyday tasks. Quantum computers are specialized tools for specific types of problems. You'll still use a regular computer for homework, games, and browsing the internet.

**Q: How can something be 0 and 1 at the same time?**
> A: It's genuinely strange! In the quantum world, particles behave differently than objects we can see. Scientists describe it mathematically, but even they find it weird. The important thing is that it *works* — and we can use it.

**Q: Can I get a quantum computer at home?**
> A: Not yet — they need to be kept extremely cold (colder than outer space!) and are very expensive. But you can access them through the cloud, just like we did today!

**Q: Is quantum computing related to quantum physics?**
> A: Yes! Quantum computing uses the strange rules of quantum physics — the physics of very tiny things like atoms and electrons — to process information in new ways.

---

## Resources

### For Students
- [IBM Quantum Learning](https://learning.quantum.ibm.com/) — Free courses and tutorials
- [Quantum TiqTaqToe](https://quantumtictactoe.com/play) — The game we played in class

### For Teachers
- [Q-12 Education](https://q12education.org/) — Resources for teaching quantum in K-12
- *"Quantum Computing: A Gentle Introduction"* by Eleanor Rieffel and Wolfgang Polak
- [Qubit by Qubit](https://www.qubitbyqubit.org/) — Free quantum computing courses for students

---

## Final Notes for Teachers

**Preparation:**
- Run through the entire notebook yourself before class
- Test the Quantum Tic-Tac-Toe game on your school's network
- Have your IBM Quantum API token ready

**Mindset:**
- It's okay not to know everything — quantum physics is genuinely confusing, even for experts
- Focus on the *concepts* and *excitement*, not the math
- Celebrate that students are doing something cutting-edge!

**Timing:**
- The 90-minute timing is flexible — feel free to skip or shorten activities if needed
- The quantum computer wait time is unpredictable; have backup discussion topics ready

---

**Enjoy exploring the quantum realm with your students!** 🚀
