# Quantum Communication with Qiskit

This repository contains implementations of quantum communication protocols using Qiskit.

## 1. Quantum Teleportation

Quantum teleportation transfers an unknown quantum state from Alice to Bob using a shared entangled Bell pair and two classical bits.

The implementation includes:
- Bell-pair preparation
- Random quantum-state preparation
- Alice's Bell-basis measurement
- Classical communication
- Bob's correction operations
- Statevector verification

See `quantum-teleportation.ipynb` for the full implementation.

---

## 2. Superdense Coding

Superdense coding allows Alice to send **two classical bits by transmitting only one qubit**, provided that Alice and Bob already share an entangled Bell pair.

The implementation includes:
- Bell-pair preparation
- Random two-bit message generation
- Alice's encoding operations
- Bob's decoding operations
- Measurement and message recovery
- Depolarizing noise simulation
- Multi-shot simulation and success-rate analysis

See `superdense-coding.ipynb` for the full implementation.

## Requirements

- Python
- Qiskit
- Qiskit Aer
- Matplotlib