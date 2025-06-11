# Resources for SpectrumX

Support material for SpectrumX workshops, tutorials, and other events.

## Spectrogram Example

The spectrogram example demonstrates how to download DigitalRF data from the SpectrumX Data System (SDS) and create spectrograms from the data.

### Prerequisites

- Python 3.x
- Required Python packages:
  - spectrumx-client
  - digital_rf
  - h5py
  - numpy
  - matplotlib
  - scipy

> **Note:** All required dependencies are pre-installed in the SpectrumX Visualization Interface's JupyterHub instance, which is hosted at https://svi.crc.nd.edu/notebook. This is the recommended environment for running the spectrogram example.

### Setup

1. Install the required packages:
```bash
pip install spectrumx-client digital_rf h5py numpy matplotlib scipy
```

2. Get your SDS secret token from the SpectrumX portal.

### Running the Example

1. Navigate to the spectrogram example directory:
```bash
cd demos/spectrogram_from_sds
```

2. Open the Jupyter notebook:
```bash
jupyter notebook spectrogram.ipynb
```

3. In the notebook:
   - Replace `YOUR_SECRET_TOKEN` with your SDS secret token
   - Replace `/YOUR_PATH` with the path to your data in the SDS
   - Replace `data/files/YOUR_USERNAME/YOUR_PATH/` with the local path where you want to store the downloaded data

4. Run the cells in sequence to:
   - Download the DigitalRF data from the SDS
   - Process the data and generate spectrograms
   - View the resulting spectrograms

The example will create spectrograms for each channel in the downloaded data, with automatic scaling of the power levels.
