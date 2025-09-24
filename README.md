# Reinforcement Learning in ViZDoom 🎮 AI Research & Tools Project

**Grade Received: 10/10**  

## 📌 Project Overview

This project explores reinforcement learning in complex, dynamic environments using the **ViZDoom** simulation platform. The core aim is to build and optimize end-to-end RL agent pipelines in **Python** on **Ubuntu Linux**, incorporating **computer vision**, **Curriculum Learning**, and **Large Language Models (LLMs)** for automated reward shaping. The result is a robust system that trains agents more efficiently, adapts quicker, and delivers improved performance across multiple scenarios.

---

## 🧠 Key Features & Innovations

- **Modular RL Pipelines:** Full data → training → evaluation pipelines in Python  
- **Linux-based Setup:** Developed in Ubuntu for real-world deployment relevance  
- **Curriculum Learning:** Progressive difficulty scheduling to stabilize learning  
- **LLM-based Reward Shaping:** Automated reward function design to reduce manual tuning  
- **Vision + Control:** Agents use CNN-based perception layers to interpret game state  
- **Scenarios Covered:** Basic, Deadly Corridor, Defend the Center, Defend the Line  

---

## 🛠️ Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Dimitris-Anagnostopoulos/Thesis_2023-2024.Reinforcement_Learning_ViZDoom.git
   cd Thesis_2023-2024.Reinforcement_Learning_ViZDoom
   ```

2. **Setup Environment (Python 3.9 with Conda):**
   ```bash
   conda create --name doom_env python=3.9
   conda activate doom_env
   pip install -r Other/requirements.txt
   ```

3. **ViZDoom dependency:**
   ```bash
   git clone https://github.com/Farama-Foundation/ViZDoom.git
   ```

4. **Run in training or test mode:**
   ```bash
   python main.py -lvl <LEVEL> -m <mode> -t <technique> [-mdl <model>] [-eps <episodes>] [-r] [-d]
   ```
   Use `-h` or `--help` for command-line options.

5. **Run all techniques across scenarios:**
   ```bash
   ./superset.sh
   ```

6. **View training metrics:**
   ```bash
   tensorboard --logdir Data/Logs/
   ```

---

## 📊 Project Architecture

```
Data & Logs
  ├── Training data & model checkpoints  
  └── TensorBoard logs  
Training
  ├── main.py  
  ├── agent modules  
  └── reward modules  
Models & Vision
  ├── CNN architectures  
  └── Vision preprocessing modules  
Other
  ├── Display utilities (map layout, agent view)  
  └── Scripts & configuration files  
```

---

## 🧩 Technical Stack & Tools

| Component | Tools / Libraries |
|----------|--------------------|
| Language | Python 3.9 |
| OS / Environment | Linux (Ubuntu) |
| RL Algorithm | PPO (Proximal Policy Optimization) |
| Vision / Perception | Convolutional Neural Networks (CNNs) |
| Reward Design | Large Language Models (LLMs) - e.g. GPT-based |
| Learning Techniques | Curriculum Learning |
| Logging & Monitoring | TensorBoard |
| Environment | ViZDoom simulation |
| Dependency Management | Conda, pip |
| Version Control | Git |

---

## 🏆 Results & Insights

- Curriculum Learning reliably improved training stability and reduced convergence time.  
- LLM-based reward shaping automated parts of the reward function design, making agents more adaptable with less manual tuning.  
- Demonstrated meaningful performance gains across multiple ViZDoom scenarios (e.g. “Defend the Center,” “Deadly Corridor”).  


---

## 📄 License & Attribution

Original ViZDoom environment and dependencies by the **Farama Foundation**.  

---

## 📬 Contact & Further Work

- GitHub: [Dimitris-Anagnostopoulos](https://github.com/Dimitris-Anagnostopoulos)  
- LinkedIn: [Dimitris Anagnostopoulos](https://www.linkedin.com/in/dimitris-anagnostopoulos-396361241/)  

Feel free to explore the code, run experiments, or reach out with suggestions or questions.  
