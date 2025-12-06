# Quantum Computing Terminology Cheat Sheet

## The Basics

- **Qubit**: The basic unit of quantum information. Unlike a regular bit (which is either 0 or 1), a qubit can be 0, 1, or *both at the same time*. Think of it as a coin that can be heads, tails, or spinning in the air.

- **Superposition**: When a qubit is in both 0 and 1 at the same time. It's like that spinning coin — it's not heads or tails until you look at it. This lets quantum computers explore many possibilities at once.

- **Entanglement**: A special link between two or more qubits where they become connected. When you measure one entangled qubit, you instantly know something about the other — even if they're on opposite sides of the universe! Einstein called this "spooky action at a distance."

## Gates (Quantum Operations)

- **Gate**: An operation that changes the state of a qubit. Gates are like instructions that tell qubits what to do. Common gates include:

  - **Hadamard (H) Gate**: Puts a qubit into superposition — like flipping a coin into the air.

  - **X Gate**: Flips a qubit from 0 to 1 or from 1 to 0. Also called a NOT gate or "bit flip."

  - **Controlled-X (CX or CNOT) Gate**: A two-qubit gate that flips the second qubit *only if* the first qubit is 1. This is the key gate for creating entanglement.

## Measurements

- **Observable**: A way to measure qubits to get information out of a quantum circuit. Different observables ask different "questions" about the qubits:
  - **Z observable**: Asks "is this qubit 0 or 1?"
  - **X observable**: Asks "is this qubit in the + or - superposition?"
  - **ZZ or XX**: Asks "how are these two qubits related to each other?"

- **Shots**: The number of times you run a quantum circuit. Since quantum results are probabilistic (like rolling dice), running more shots gives you a better average. Typical values are 1000 or more.

## Technical Terms

- **Phase**: The "angle" of a qubit's quantum state. You can't see it directly, but it affects how qubits interact with each other. Think of it like the timing of a wave.

- **Estimator**: A tool that runs your circuit many times, collects all the measurements, and calculates the average result. It helps turn noisy quantum data into useful answers.

- **Backend**: The actual quantum computer (or simulator) that runs your circuit. When you use IBM Quantum, you're connecting to real quantum computers in labs around the world.

- **Noise**: Random errors that happen in quantum computers. Qubits are extremely sensitive — even tiny vibrations or temperature changes can cause mistakes. That's why we run circuits many times and average the results.

- **Job ID**: A unique code for your submitted quantum program. Since quantum computers are shared by many users, your job goes into a queue. The Job ID lets you check on your job's status or get your results later.

## Quick Reference

| Term | One-Line Summary |
|------|------------------|
| Qubit | A quantum bit that can be 0, 1, or both |
| Superposition | Being in multiple states at once |
| Entanglement | Qubits linked so measuring one affects the other |
| H Gate | Creates superposition |
| X Gate | Flips 0↔1 |
| CX Gate | Flips second qubit if first is 1 |
| Shots | Number of times to run the circuit |
| Noise | Random errors in quantum computers |
