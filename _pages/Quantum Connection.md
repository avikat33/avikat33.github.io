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

The main VQE equation is:

$$
E(\theta)=\langle\psi(\theta)|H|\psi(\theta)\rangle
$$

where:

- \(E(\theta)\) represents the energy of the current quantum state.
- \(|\psi(\theta)\rangle\) represents the trial wave function created by a parameterized quantum circuit.
- \(\theta\) represents the adjustable parameters (the "knobs") of the quantum circuit.
- \(H\) is the Hamiltonian, which represents the total energy of the system.
- \(\langle\psi(\theta)|H|\psi(\theta)\rangle\) calculates the expected energy of the state.

VQE works by repeatedly adjusting the parameters \(\theta\) to minimize the energy. The lowest energy found corresponds to the most stable state of the molecule or material.

Youtube Video to help understand VQE: 

<a href="https://www.youtube.com/watch?v=TUFovZsBcW4">
<img src="https://img.youtube.com/vi/TUFovZsBcW4/maxresdefault.jpg" 
alt="Quantum Computing Video Preview">
</a>

### Quantum Annealing
Quantum annealing is a quantum computing method designed to solve complex optimization problems by finding the best solution among many possible choices. It uses quantum effects such as superposition and quantum tunneling to explore different solutions more efficiently. At the beginning of the process, qubits are placed into a superposition state, allowing the system to represent many possible solutions at the same time.

During the annealing process, quantum tunneling allows the system to move through energy barriers and avoid solutions that are not optimal. Unlike classical methods that may get stuck in a local minimum, quantum annealing can explore different possibilities to search for a better solution. As the process continues, the quantum state evolves until the system reaches a final state that represents the best solution.

Quantum annealing problems are often represented using the Ising model, which converts an optimization problem into an energy equation. In this model, variables represent possible choices, hi​ represents the effect of individual choices, and Ji​ represents interactions between choices. The goal is to find the combination of choices that produces the lowest energy solution.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap;">

  <figure>
    <img src="/assets/images/an.png" width="200">
  </figure>

  <figure>
    <img src="/assets/images/an2.png" width="200">
    <figcaption><em>Annealing process’s energy diagram shows raising the energy barrier for a single qubit, resulting in a 50/50 probability of ending in a classical state of 0 or 1. Figure from D-Wave quantum</em></figcaption>
  </figure>

</div>

### Ising Model 

The Ising model is a mathematical model used to represent optimization problems as an energy equation. It was used to study magnetic materials,which can either have spin up (+1) or spin down (-1). These states can represent possible choices or variables in an optimization problem.

The Ising energy equation is:

$$
E(s)=\sum_{i=1}^{N} h_i s_i+\sum_{i=1}^{N}\sum_{j=i+1}^{N}J_{ij}s_is_j
$$

What the variables mean: 
where:

- \(s_i\) represents the state of each variable, either \(+1\) or \(-1\).
- \(h_i\) represents the individual effect or preference of each variable.
- \(J_{ij}\) represents the relationship between two variables, showing whether they should work together or oppose each other.
- \(E(s)\) represents the total energy of a possible solution.

For alloy design, the Ising model can represent different choices of elements and their positions within a crystal structure. Each variable can represent whether a specific element occupies a certain location, while the interactions between variables describe how neighboring atoms influence each other. Overall goal is to find the most stable configuration. 
