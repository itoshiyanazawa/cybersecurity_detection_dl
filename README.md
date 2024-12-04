# Cyber Threat Detection using Deep Learning

## Project Overview

This project aims to develop a deep learning model for detecting cyber threats using the BETH dataset. As cyber attacks become increasingly sophisticated, traditional threat detection methods often fall short. Our model leverages deep learning techniques to analyze vast amounts of data and identify patterns that may not be immediately obvious to human analysts, enhancing cybersecurity measures for organizations[1].

## Dataset

We use the BETH dataset, which simulates real-world logs and provides a rich source of information for training and testing our model. The dataset has undergone preprocessing and includes a target label, `sus_label`, indicating whether an event is malicious (1) or benign (0)[1].

### Data Description

| Column | Description |
|--------|-------------|
| processId | Unique identifier for the process that generated the event (int64) |
| threadId | ID for the thread spawning the log (int64) |
| parentProcessId | Label for the process spawning this log (int64) |
| userId | ID of user spawning the log (int64) |
| mountNamespace | Mounting restrictions the process log works within (int64) |
| argsNum | Number of arguments passed to the event (int64) |
| returnValue | Value returned from the event log (usually 0) (int64) |
| sus_label | Binary label for suspicious event (1 is suspicious, 0 is not) (int64) |

## Requirements

- Python 3.x
- pandas
- scikit-learn
- PyTorch
- torchmetrics


## Model Architecture

Our deep learning model is designed to process the features from the BETH dataset and output a binary classification indicating whether an event is suspicious or not. The specific architecture details will be provided in the code documentation.

## Performance
The model has achieved 90% accuracy on the testing sample, demonstrating its effectiveness in detecting cyber threats.

## Contributing

Contributions to improve the model's performance or extend its capabilities are welcome. Please feel free to submit pull requests or open issues for discussion.
