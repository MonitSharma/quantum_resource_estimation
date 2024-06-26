# Quantum Resource Estimation


### What is Quantum Resource Estimation (QRE)?

QRE provides estimates on what it would take to accurately run an algorithm:
1. T Gate Count
2. Logical Qubit Count
3. Rotational Gate Count
4. Physical Qubit Count
5. Clifford Gate Count : Hadamard (H), Phase (S) and Controlled Not (CNOT)
6. Runtime 


### Why is it important?
<li> Gives an idea of how close/far current hardware is</li>
<li> Illustrates trade offs (time/space(or number of qubits))</li>
<li> Allows for comparisons between implementations.</li>


### Current Tools

1. [MIT pyLIQTR](https://github.com/isi-usc-edu/pyLIQTR)
2. [Google's Qualtran](https://github.com/quantumlib/Qualtran)
3. [Zapata AI's BenchQ](https://github.com/zapatacomputing/benchq)
4. [Microsoft's Azure QRE](https://learn.microsoft.com/en-us/azure/quantum/intro-to-resource-estimation) and [this](https://github.com/microsoft/Quantum/tree/main/samples/azure-quantum/resource-estimation)

   


