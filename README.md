# Vanguard AI: Enterprise-Grade Temporal Event Intelligence

Vanguard AI is a sophisticated framework designed for the autonomous forecasting of global events using Large Language Model (LLM) agents. By integrating structured Knowledge Graphs (KG) with unstructured news intelligence, Vanguard leverages a refined **ReAct (Reasoning and Acting)** architecture to synthesize predictive insights with high temporal precision.

---

## 🏛 Architecture & Methodology

Vanguard AI operates on a decoupled architecture that separates decision-making logic from data acquisition and evaluation.

### Core Components
- **Forecasting Engine (`src/engine`)**: Orchestrates the multi-step reasoning process, utilizing dynamic prompt engineering and iterative thought loops.
- **Knowledge Core (`src/core`)**: A specialized interface for the GDELT GKG (Global Knowledge Graph), providing high-fidelity relational data.
- **Intelligence Pipeline (`src/pipeline`)**: An end-to-end suite for downloading, cleaning, and encoding multi-source textual data.
- **Evaluation Suite (`src/evaluator`)**: Implements rigorous benchmarking metrics including Macro/Micro F1, KL-Divergence, and temporal accuracy analysis.

---

## 🚀 Intelligent Agent Strategies

Standard forecasting traditional models often fail in complex geopolitical scenarios. Vanguard employs advanced agentic patterns:

1. **ReAct Loop**: Agents iteratively think, act (using customized APIs), and observe results to refine their hypothesis before delivering a final forecast.
2. **Multi-Source Synthesis**: Simultaneous querying of historical relations and real-time news articles to eliminate bias.
3. **Temporal Reasoning**: Specialized logic to handle varying forecasting horizons, from short-term shifts to long-term strategic trends.

---

## 🛠 Installation

### System Requirements
- **OS**: Linux / Windows / macOS
- **Environment**: Python 3.9 or higher
- **Resources**: CUDA-compatible GPU recommended for local inference

### Setup
```bash
# Clone the repository
git clone https://github.com/jamarius-fortson/Vanguard-AI-Agent.git
cd Vanguard-AI-Agent

# Initialize environment
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate

# Install production dependencies
pip install -r requirements.txt
pip install flash-attn --no-build-isolation
```

---

## ⚡ Usage Execution

### Running the Forecasting Agent
Navigate to the engine directory and execute the primary agent script:

```bash
cd src/engine
python react_agents.py --model_name gpt-4o-2024-05-13 --action block --api full
```

### Strategic Parameters
- `--model_name`: Supports `gpt-4o`, `gpt-4-turbo`, `Mistral-7B`, and `Llama-3`.
- `--timediff`: Set the temporal forecasting window (default: 1 day).
- `--max_steps`: Control the depth of the reasoning process (default: 20 steps).

---

## 📊 Benchmarking & Performance

Vanguard AI is evaluated against global event datasets derived from the **GDELT Project**, focusing on international relations forecasting.

| Metric | Vanguard AI (ReAct) | Baseline (Direct IO) |
| :--- | :--- | :--- |
| **Relation F1** | High | Low |
| **Reasoning Depth** | 20+ Steps | 0 Steps |
| **Data Fidelity**| Multi-Source | Single-Source |

---

## 📜 Scientific Citation

This framework is based on the methodology proposed in:
> **MIRAI: Evaluating LLM Agents for Event Forecasting** (2024).

```bibtex
@misc{ye2024vanguardevaluatingllmagents,
      title={Vanguard AI: Evaluating LLM Agents for Event Forecasting}, 
      author={Chenchen Ye and Ziniu Hu and Yihe Deng and Zijie Huang and Mingyu Derek Ma and Yanqiao Zhu and Wei Wang},
      year={2024},
      eprint={2407.01231},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

---

## 🛡 License & Disclaimer

Released under the **MIT License**. Data extracted from the GDELT Project is used in accordance with their terms of service. This tool is intended for research and analytical intelligence purposes.

---
**Vanguard AI Research Team** | *Deciphering the Future through Agentic Intelligence*
