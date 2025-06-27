# GPU-Accelerated Information Spread on Twitter Ego Network

This project demonstrates how to analyze and simulate information spread in a large-scale social network using GPU-accelerated libraries. The workflow leverages RAPIDS cuGraph/cuDF for fast graph analytics and Graphistry for interactive visualization.

## What This Project Does
- Loads and preprocesses the Twitter Ego Network dataset (over 800,000 edges)
- Computes key network metrics (nodes, edges, degree, components)
- Visualizes the network interactively with Graphistry
- Simulates information spread using a simple contagion model
- Compares different seeding strategies (random, degree, PageRank, community-based)
- Plots the results for analysis and comparison

## Replication Steps
1. **Requirements**
   - NVIDIA GPU with CUDA support
   - Python 3.8+
   - [RAPIDS cuGraph/cuDF](https://rapids.ai/), [Graphistry](https://www.graphistry.com/), pandas, seaborn, matplotlib

2. **Install Dependencies**
   Run the following in your terminal or the first notebook cell:
   ```sh
   pip install --upgrade pip
   pip install cudf-cu11 cugraph-cu11 cupy-cuda11x graphistry pandas matplotlib seaborn --extra-index-url=https://pypi.nvidia.com
   ```

3. **Download the Dataset**
   - Download `twitter_combined.txt` from [SNAP Datasets](https://snap.stanford.edu/data/egonets-Twitter.html)
   - Place it in the same directory as the notebook

4. **Set Up Graphistry**
   - Register for a free API key at [Graphistry Hub](https://hub.graphistry.com/)
   - Set your API key as an environment variable `GRAPHISTRY_API_KEY` or directly in the notebook

5. **Run the Notebook**
   - Open `Copy_of_MSML606_Final_code_GPU.ipynb`
   - Run all cells in order

## Citation
If you use this code or notebook, please cite the original [Twitter Ego Network dataset](https://snap.stanford.edu/data/egonets-Twitter.html) and acknowledge RAPIDS cuGraph and Graphistry.

---

For questions or suggestions, feel free to open an issue or pull request.
