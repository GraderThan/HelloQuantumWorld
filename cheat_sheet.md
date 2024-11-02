# Quantum Computing Terminology Cheat Sheet

- **Qubit**: The basic unit of quantum information, similar to a classical bit but can represent 0, 1, or both at the same time (superposition).

- **Superposition**: A state where a qubit can be in a combination of both 0 and 1, allowing quantum computers to process more information simultaneously.

- **Entanglement**: A special connection between two or more qubits where the state of one qubit instantly influences the other(s), even if they are separated.

- **Gate**: An operation that changes the state of a qubit, similar to logic gates in classical computing. Common gates include:
  - **Hadamard (H) Gate**: Puts a qubit into a superposition state.
  - **X Gate**: Flips a qubit from 0 to 1 or from 1 to 0 (also called a NOT gate).
  - **Controlled-X (CX) Gate**: A gate that flips the target qubit only if the control qubit is 1. This is essential for creating entanglement.

- **Phase State**: The "angle" of a qubit’s state around the Z-axis of the Bloch sphere. Phase doesn’t affect whether a qubit is 0 or 1 but influences how it interacts with other qubits.

- **Flip State**: Indicates whether a qubit is in state 0 or 1. The X gate (or "flip" gate) changes the qubit's state between 0 and 1.

- **Observable**: A specific measurement set up in a quantum circuit to gather data from qubits. Different observables (like "ZZ" or "XX") help measure various properties of qubits.

- **Estimator**: A tool that calculates the expected (average) result from multiple measurements of a circuit, giving a reliable outcome from potentially noisy quantum data.

- **Shots**: The number of times a quantum circuit is run to gather data. More shots reduce randomness and provide more accurate results.

- **Backend**: The actual quantum computer or simulator where the quantum circuit runs. In cloud quantum computing, users share access to backends around the world.

- **Noise**: Unwanted errors in a quantum computer caused by interference, hardware issues, or environmental factors. Noise can make results less accurate, so circuits are often run many times to get more reliable answers.

- **Job ID**: A unique identifier for a submitted quantum job, allowing users to track and retrieve their results once the quantum computer has finished processing.