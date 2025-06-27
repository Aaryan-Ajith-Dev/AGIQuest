# AGIQuest

# AGI Race Multi-Agent Reinforcement Learning

This repository contains a series of increasingly complex environments simulating AGI research race dynamics using multi-agent reinforcement learning. The environments model strategic decision-making in competitive and collaborative scenarios, incorporating features such as team management, resource allocation, and probabilistic AGI discovery.

## Repository Structure

- `Version_1`: Basic single-agent environment with AGI exploration
- `Version_2`: Single-agent environment with team management
- `Version_3`: Simple Multi-agent environment with a dummy collaborator
- `Version_4`: Multi-agent environment with a dummy collaborator and hiring firing
- `Version_5`: Simple True multi-agent competitive environment 
- `Version_6 `: True multi-agent competitive environment with hiring firing

## Installation

### Using Conda (Recommended)

1. Clone the repository:
```bash
git clone https://github.com/standing-on-giants/AGIQuest.git
```

2. Create a new conda environment:
```bash
conda create -n agi-race python=3.9
conda activate agi-race
```

3. Install the required dependencies:
```bash
conda install -c conda-forge numpy matplotlib pytorch gymnasium tqdm ipykernel
conda install -c pytorch pytorch
pip install "gymnasium[all]"
```

4. Register the environment in your Jupyter notebook:
```bash
python -m ipykernel install --user --name=agi-race --display-name="Python (AGI Race)"
```

### Using pip

If you prefer not to use conda, you can install the dependencies using pip:

```bash
pip install numpy matplotlib torch gymnasium tqdm jupyter
pip install "gymnasium[all]"
```

### Running an example notebook

An example notebook is `Version6_complete.ipynb`. To run this notebook:

1. Ensure your conda environment is activated:
```bash
conda activate agi-race
```

2. Launch Jupyter Notebook:
```bash
jupyter notebook
```

3. Open `Version6_complete.ipynb` and select the `agi-race` kernel.

4. Run all cells to:
   - Initialize the environment
   - Create the agent preprocessor
   - Initialize DQN agents
   - Train the agents


## Report
- A detailed analysis can be found in the following ![report](./RL_Report.pdf).

