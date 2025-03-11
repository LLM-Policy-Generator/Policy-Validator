# Policy Consistency Validation Notebook

This notebook validates generated IDS policies against the expected IDS ontology. It is organized into the following sections:

- **Setup & Imports:** Import libraries and set paths.
- **Data Loading:** Load the generated policies from an Excel file.
- **Validation Functions:** Define functions to validate the policy JSON structure.
- **Policy Validation:** Apply validation to each generated policy.
- **Validation Summary:** Summarize and visualize the validation results.
- **Conclusion:** Final remarks and next steps.

## Overview

The Policy Consistency Validation Notebook is designed to ensure that generated IDS policies conform to the required ontology structure. It:
- Loads policies from an Excel file.
- Uses custom functions to validate the structure and content of each policy.
- Displays validation results and provides visual summaries of valid versus invalid policies.
- Offers insights into potential improvements in the policy generation process.

## Prerequisites

- **Python 3.7+**
- **Jupyter Notebook** or **JupyterLab**

### Required Python Libraries

- `os`
- `json`
- `re`
- `time`
- `pandas`
- `matplotlib`

You can install the required libraries using pip:

```
pip install pandas matplotlib
```

### Setup
1. Data File:
Ensure your generated policies are stored in an Excel file named Generated_Policies.xlsx. If your file is located elsewhere or named differently, update the data_file variable in the notebook accordingly.
2. Data Format:
The Excel file should contain:
- A column (e.g., Policy) with the original policy description.
- A column (e.g., Generated_Policy) containing the generated policy as a JSON-formatted string.

Running the Notebook
1. Launch Jupyter Notebook or JupyterLab.
2. Open the Policy_Consistency_Validation.ipynb notebook.
3. Run all cells sequentially:
- The notebook will load the data.
- Validate each generated policy using the defined functions.
- Display a sample of the results and a bar chart summarizing the validation status.

### Contributing

Contributions are welcome! Please follow the existing code style and documentation guidelines when submitting improvements or fixes.

### License

This project is licensed under the MIT License. See the LICENSE file for details.

### Acknowledgements

This project is part of a research effort on IDS policy generation and validation for a conference paper. Special thanks to all contributors and reviewers for their valuable feedback.
