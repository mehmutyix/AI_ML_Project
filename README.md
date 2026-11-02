# Multi-Agent Shipment Exception Resolution

A LangChain and LangGraph notebook project that classifies shipment delivery events, selects resolution actions, and generates customer communications. The completed notebook includes saved test results and evaluation metrics.

## Project files

- `Project_3_Full_CODE_MultiAgentMAI_completed.ipynb` - completed notebook with saved outputs.
- `Project_3_Full_CODE_MultiAgentMAI_completed_full_output.html` - static HTML export of the notebook and its saved outputs.
- `Project_3_Full_CODE_MultiAgentMAI.ipynb` - original notebook.
- `delivery_logs.csv`, `ground_truth.csv`, `customers.db`, `customers.zip`, and `exception_resolution_playbook.pdf` - test inputs and reference material.
- `requirements.txt` - Python dependencies.

## Setup

1. Use Python 3.12 for the pinned package versions.
2. Create and activate a virtual environment, then install dependencies:

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   python -m pip install -r requirements.txt
   ```

3. Copy `config.example.json` to `config.json` and enter your own API credentials and API base URL. `config.json` is intentionally ignored by Git and must never be committed.
4. Open the completed notebook in VS Code or Jupyter and run its cells.

The notebook can use an OpenAI-compatible API and optionally LangSmith tracing. Supply credentials for the services you enable. Do not put credentials in notebook cells, outputs, or source control.

## Results

The completed notebook reports 100% task completion on its included test cases. Escalation accuracy is 75% across the eight cases with escalation labels; review those results before using the workflow in production. These results are from a small test dataset and are not a production performance guarantee.
