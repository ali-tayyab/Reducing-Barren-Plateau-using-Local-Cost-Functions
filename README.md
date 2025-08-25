## **Quantum Weather Forecasting**

### **Project Overview**
During my participation at **WISER 2025**, I worked on exploring **quantum computing approaches for weather forecasting**. Traditional weather prediction relies on **non-linear partial differential equations (PDEs)**, which are computationally intensive and not directly compatible with current quantum hardware.  

To bridge this gap, I implemented a **quantum-ready workflow**:

1. **Linearization of Non-linear PDEs**  
   - Applied techniques such as **Carleman linearization** to convert non-linear PDEs into an **infinite set of linear ordinary differential equations (ODEs)**.  
   - This approach allowed us to represent the dynamics in a form suitable for **quantum simulation**, though truncation was necessary for practical implementation, introducing controlled approximation errors.

2. **Quantum Simulation of Linearized ODEs**  
   - Addressed the **quantum data-loading challenge** for large N $\times$ N matrices using **Linear Combination of Unitaries (LCU) and decomposition techniques**.  
   - Enabled simulation of truncated ODE systems while keeping classical-quantum resource requirements manageable.

3. **Mitigation of Barren Plateaus**  
   - During variational quantum circuit training, I encountered **barren plateau phenomena**, where gradients vanish exponentially with the number of qubits, making optimization infeasible.  
   - I **implemented local cost functions** using **Pennylane**, effectively alleviating the barren plateau problem and allowing stable gradient-based training for larger qubit systems.  
   - This demonstrated **algorithmic rigor** and practical **quantum optimization under realistic constraints**.

#### **Achievements**
- Reduced the impact of barren plateaus in variational quantum circuits for weather forecasting models.

#### **Tools & Libraries**
- **PennyLane** for quantum circuit implementation and gradient computation.  
- **NumPy** and **Matplotlib** for classical preprocessing, simulation, and analysis.  
