---
title: "3. Quantum Connection"
permalink: /quantum-connection/
layout: single
author_profile: true
---

## 3.1 How Does Quantum Computing Help?

### Variational Quantum Eigensolver (VQE)s

The Variational Quantum Eigensolver (VQE) is a quantum algorithm used to find the lowest energy state of a molecule or material. It combines a quantum computer with a classical computer to solve complex energy problems.

The Variational Method uses a trial wave function, called an ansatz, with adjustable values called parameters. These parameters act like knobs that can be changed to search for the true lowest-energy state of a system. The Eigensolver finds the energy levels of a system by solving for the eigenvalues of the Hamiltonian, which is the mathematical operator that describes the energy of the system. The lowest energy level represents the most stable state.

In VQE, the quantum computer creates a possible state of the molecule and calculates its energy using the Hamiltonian. A classical computer then adjusts the parameters of the quantum circuit to find a state with lower energy. This process repeats until the algorithm finds the lowest possible energy state, helping scientists predict the stability and properties of materials.

### Quantum Annealing
Quantum annealing is a quantum computing method designed to solve complex optimization problems by finding the best solution among many possible choices. It uses quantum effects such as superposition and quantum tunneling to explore different solutions more efficiently. At the beginning of the process, qubits are placed into a superposition state, allowing the system to represent many possible solutions at the same time.

During the annealing process, quantum tunneling allows the system to move through energy barriers and avoid solutions that are not optimal. Unlike classical methods that may get stuck in a local minimum, quantum annealing can explore different possibilities to search for a better solution. As the process continues, the quantum state evolves until the system reaches a final state that represents the best solution.

Quantum annealing problems are often represented using the Ising model, which converts an optimization problem into an energy equation. In this model, variables represent possible choices, hi​ represents the effect of individual choices, and Ji​ represents interactions between choices. The goal is to find the combination of choices that produces the lowest energy solution.
