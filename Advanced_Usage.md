- [Basic things to do for an experiment](#basic-things-to-do-for-an-experiment)
- [1. Initialize](#1-initialize)
  - [How to Initialize a qubit ?](#how-to-initialize-a-qubit-)
  - [How to initialize without circuit ?](#how-to-initialize-without-circuit-)
- [2. Drawing Circuits](#2-drawing-circuits)
  - [How to add gates in a quantum circuit ?](#how-to-add-gates-in-a-quantum-circuit-)
  - [How to add 2/3 qubit gates in a quantum circuit ?](#how-to-add-23-qubit-gates-in-a-quantum-circuit-)
  - [How to measure a qubit ?](#how-to-measure-a-qubit-)
  - [How to apply a conditional gate based on a classical measurement ?](#how-to-apply-a-conditional-gate-based-on-a-classical-measurement-)
- [3. Connecting to Backend/device/simulator](#3-connecting-to-backenddevicesimulator)
- [4. How to retrieve results after experiment](#4-how-to-retrieve-results-after-experiment)
- [5. How to plot data](#5-how-to-plot-data)

# Basic things to do for an experiment

# 1. Initialize

## How to Initialize a qubit ?
1. Create the Circuit
2. use the initializer function = `circuit.initialize([a,b],which_qubit)` where a,b are coefficients of 0 and 1 respectively for a initial state $a|0\rangle + b|1\rangle$

- By default its all qubits are initialized to $|0\rangle$ state
- for a superposition add a Hadamard gate to get  $\frac{1}{\sqrt{2}}(|0\rangle + |1\rangle)$ state

## How to initialize without circuit ?
1. use `sv = Statevector.from_label('000')` = to create a labelled state $|000\rangle$
2. use `sv.evolve(circuit)` = to evolve the qubits based on a circuit then plot the results
3. get the data using `sv.data`
4. plot it using the visualization tools

# 2. Drawing Circuits

## How to add gates in a quantum circuit ?


## How to add 2/3 qubit gates in a quantum circuit ?


## How to measure a qubit ?


## How to apply a conditional gate based on a classical measurement ?


# 3. Connecting to Backend/device/simulator
**NOTE : You can run experiments only until you have credits , once credits run out you cannot submit jobs. Credits get refreshed after a job completes**

# 4. How to retrieve results after experiment 



# 5. How to plot data