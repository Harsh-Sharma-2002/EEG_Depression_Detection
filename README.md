# EEG-Based Depression Detection and Brain-Controlled Interfaces

This project leverages advanced machine learning techniques to analyze EEG data for detecting depression and exploring potential applications in brain-machine interfaces. It demonstrates a novel approach combining **Graph Convolutional Networks (GCN)** for spatial EEG data analysis and **Gated Recurrent Units (GRU)** for time-series modeling.

## Objectives
- **Depression Detection:** Develop a robust system for identifying patterns in EEG data associated with depression.
- **Future Applications:** Lay the groundwork for enabling individuals with disabilities to control machines through brain signals.

## Key Features
- **Graph-Based Representation:** Utilizes GCN to model the spatial connectivity of EEG electrode data.
- **Temporal Insights:** GRU effectively captures the sequential dynamics of EEG signals.
- **Scalability:** The architecture can adapt to diverse EEG-based applications beyond depression detection.

## Methodology
### 1. Data Preprocessing
- **Bandpass Filtering:** Filters EEG signals within a specific frequency range to isolate relevant brainwave activity (e.g., 0.5–50 Hz).
- **Notch Filtering:** Removes powerline noise (e.g., 50/60 Hz) to improve signal quality.
- **Data Slicing:** Segments EEG recordings into shorter, overlapping intervals to enhance temporal analysis.
- **Normalization:** Standardizes EEG values to remove biases and improve model performance.

### 2. Graph Construction
- EEG electrode locations are represented as nodes.
- Connections (edges) are established based on electrode proximity or functional connectivity.

### 3. Modeling
- GCN extracts spatial features from the graph representation.
- GRU processes the temporal patterns in the extracted features.

### 4. Evaluation
- Accuracy, precision, recall, and F1-score are used to validate model performance.

## Results
- Achieved significant accuracy in distinguishing depressive and non-depressive EEG patterns.
- Demonstrated potential for real-time EEG analysis and practical implementation.

## Future Scope
- Integrating real-time EEG monitoring for adaptive systems.
- Expanding the model to support other neurological conditions.
- Developing assistive technologies for individuals with motor impairments.

## Tools & Technologies
- Python, PyTorch, and TensorFlow
- Libraries: NumPy, Pandas, Scikit-learn, NetworkX
- Dataset: Publicly available EEG datasets for mental health studies
