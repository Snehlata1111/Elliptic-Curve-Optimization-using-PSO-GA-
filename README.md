# System-Specific Elliptic Curve Optimization  

## Project Overview  
This project implements **dynamic elliptic curve generation** optimized for different system requirements such as IoT, balanced systems, and high-security applications. By combining a **two-stage neural network pipeline (Net1 & Net2)** with a **Genetic Algorithm (GA)**, the system generates and selects elliptic curves tailored to constraints like speed, memory, and security.  

The goal is to move beyond static ECC standards and design adaptive curves that deliver better performance across diverse environments.  

---

## Features  
- Two-stage neural network pipeline for curve evaluation and refinement.  
- Genetic Algorithm (GA) to evolve a population of elliptic curves and select the fittest.  
- Fitness function defined by system constraints such as execution time, memory use, and security strength.  
- Dynamic ECC generation tailored to IoT, balanced, and high-security applications.  
- Improved cryptographic performance compared to fixed ECC curves.  

---

## Methodology  

1. **Initialization**  
   Generate a random population of elliptic curves with varied parameters.  

2. **Fitness Evaluation**  
   Evaluate each curve using performance metrics (execution time, stability, and cryptographic strength).  

3. **Selection**  
   Use Tournament Selection and Roulette Wheel Selection to pick parent curves.  

4. **Neural Network Pipeline**  
   - **Net1**: predicts curve viability from population.  
   - **Net2**: fine-tunes selected curves for optimized parameters.  

5. **Evolution**  
   Apply crossover and mutation to generate the next population until optimal curves emerge.  

---

## Architecture  


---

## Results  

The system was tested across three environments:  

- **Low Power (IoT systems):** optimized for lightweight operations with minimal resource use.  
- **Balanced Systems:** trade-off between performance and cryptographic strength.  
- **High-Security Systems:** optimized for maximum strength, tolerating higher resource usage.  

---

## Tech Stack  
- **Languages:** Python  
- **Libraries:** NumPy, SciPy, PyTorch, Matplotlib  
- **Methods:** Neural Networks (MLP/LSTM), Genetic Algorithms  

---

## How to Run  

```bash
# Clone the repository
git clone https://github.com/yourusername/ecc-optimization.git
cd ecc-optimization

# Install dependencies
pip install -r requirements.txt

# Run the training
python src/train_ga_nn.py
