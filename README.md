# Quantum Teleportation with Qiskit

Implementation and simulation of the quantum teleportation protocol using Qiskit.

## Overview

This project demonstrates the teleportation of an arbitrary single-qubit state

|ψ⟩ = α|0⟩ + β|1⟩

from Alice to Bob using an entangled Bell pair and two classical bits.

The project includes:
- Preparation of a random normalized quantum state
- Bell-pair generation
- Alice's Bell-basis operations and measurements
- Bob's conditional corrections
- Simulation using Qiskit Aer
- Verification of the teleported state using quantum-state fidelity

## Teleportation Protocol

1. Alice prepares an arbitrary state |ψ⟩.
2. Alice and Bob share an entangled Bell pair.
3. Alice performs a CNOT and Hadamard operation.
4. Alice measures her two qubits.
5. The two measurement results determine Bob's corrections.
6. Bob applies the corresponding X and Z corrections.
7. Bob's qubit reproduces the original state |ψ⟩.

## Verification

The final state of Bob's qubit is compared with Alice's original state using state fidelity.

For ideal teleportation:

F = |⟨ψ_original|ψ_Bob⟩|² ≈ 1

## Requirements

- Python
- Qiskit
- Qiskit Aer
- NumPy
- Matplotlib

## Running the Project

Open the Jupyter notebook and run the cells sequentially.

The notebook:
1. Prepares Alice's state
2. Builds the teleportation circuit
3. Simulates the circuit
4. Calculates the teleportation fidelity


## Noisy Simulation

A depolarizing noise model is used to study the effect of gate errors on the teleportation protocol.

The noisy quantum state is represented using a density matrix, allowing the fidelity of Bob's received state to be compared with the ideal input state.