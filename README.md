# code-demo-Snyk
# Security Check Script with Anomaly Detection

Automates security vulnerability scanning using Snyk CLI and applies Isolation Forest for anomaly detection.

## Features
- Runs Snyk CLI (`snyk test --json`).
- Extracts vulnerability features (severity, package age, vulnerable versions).
- Detects anomalous vulnerabilities using Isolation Forest.
- Pass/fail based on critical vulnerabilities or anomalies.

## Setup

1.  **Install Prerequisites:**
    *   Python 3.6+
    *   [Snyk CLI](https://docs.snyk.io/snyk-cli/install-the-snyk-cli) (e.g., `npm install -g snyk` in Colab)
    *   Python libraries: `pip install scikit-learn requests numpy`

2.  **Authenticate Snyk:** Run `snyk auth` and follow the prompts.

## Usage

1.  Save the script code (from the notebook) as a Python file (e.g., `security_check.py`).
2.  Run the script from your project directory: `python security_check.py`
3.  The script will output the result (pass/fail) and exit with status 0 for success or 1 for failure.
