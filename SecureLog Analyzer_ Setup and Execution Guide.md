# SecureLog Analyzer: Setup and Execution Guide

This guide provides step-by-step instructions on how to set up and run the SecureLog Analyzer project on your local computer. The project is built using Python and Streamlit, offering an interactive dashboard for log analysis and threat detection.

## 1. Prerequisites

Before you begin, ensure you have the following installed on your system:

*   **Python 3.7+**: You can download Python from the official website: [python.org](https://www.python.org/downloads/)
*   **pip**: Python's package installer, which usually comes bundled with Python.

## 2. Obtain Project Files

If you have already downloaded the project files (e.g., from the previous delivery), ensure they are organized in a directory named `securelog-analyzer` with the following structure:

```
securelog-analyzer/
│
├── logs/
│ └── sample.log
│
├── utils.py
├── detector.py
├── dashboard.py
├── requirements.txt
└── README.md
```

If you haven't downloaded them yet, please refer to the previous message where the project files were attached and download them to a new directory on your computer.

## 3. Install Dependencies

Navigate to the `securelog-analyzer` directory in your terminal or command prompt and install the required Python packages using `pip`:

```bash
cd path/to/your/securelog-analyzer
pip install -r requirements.txt
```

This command will install `streamlit`, `pandas`, and `plotly`, which are essential for the dashboard's functionality.

## 4. Run the Dashboard

Once the dependencies are installed, you can launch the Streamlit dashboard from the `securelog-analyzer` directory:

```bash
streamlit run dashboard.py
```

## 5. Access the Dashboard

After running the command in step 4, Streamlit will start a local server and automatically open a new tab in your default web browser. If it doesn't open automatically, you can manually navigate to the URL displayed in your terminal (typically `http://localhost:8501`).

You should now see the SecureLog Analyzer dashboard, where you can view log summaries, visualizations, and detected threats.

## Troubleshooting

*   **`streamlit` command not found**: Ensure Streamlit is installed correctly. You might need to restart your terminal after installation.
*   **ModuleNotFoundError**: Double-check that all dependencies from `requirements.txt` are installed. Make sure you are running the commands from within the `securelog-analyzer` directory.
*   **Log file not found**: Ensure `sample.log` is present in the `logs/` subdirectory within your `securelog-analyzer` project folder.
*   
