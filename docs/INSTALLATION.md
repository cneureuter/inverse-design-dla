# Installation Guide

## Prerequisites

1. **Python Environment**
   - Python 3.7 or higher
   - pip package manager

2. **Lumerical FDTD Solutions**
   - Commercial software required for FDTD simulations
   - Valid license needed
   - lumapi Python interface

## Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/inverse-design-thesis.git
   cd inverse-design-thesis
   ```

2. **Install Python Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Verify Lumerical Installation**
   - Ensure Lumerical FDTD Solutions is installed
   - Verify lumapi is accessible from Python
   - Test with: `python -c "import lumapi"`

4. **Run Jupyter Notebooks**
   ```bash
   jupyter notebook
   ```

## Troubleshooting

- **Import Error with lumapi**: Ensure Lumerical is properly installed and licensed
- **Memory Issues**: Some notebooks require significant RAM for large simulations
- **Path Issues**: Update lumapi path in notebooks if Lumerical is installed in non-standard location

## System Requirements

- **RAM**: 8GB minimum, 16GB recommended
- **Storage**: 10GB free space for simulations
- **OS**: Windows (Lumerical compatibility)
- **Python**: 3.7+ with scientific computing packages
