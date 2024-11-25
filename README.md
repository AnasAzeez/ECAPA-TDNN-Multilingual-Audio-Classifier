
# Multilingual Audio Feature Extraction and Classification

This project provides a comprehensive pipeline for multilingual audio processing, from feature extraction to classification using the ECAPA-TDNN model.

---

## Installation

Install the required dependencies:

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu126
pip install git+https://github.com/speechbrain/speechbrain.git@develop
```

---

## Feature Extraction

1. Enter the number of file paths to load and click **"Load file paths"**.
2. Select the clips folder language by language and assign their labels.
3. Click **"Extract features"**.
4. Specify the number of files to process from each directory.

---

## Training

1. Specify the number of languages to train on and click **"Confirm"**.
2. Click **"Train and save model"**.
3. Select the feature and label files from the working directory one at a time.
4. After training, the following files will be saved in the working directory:
   - `trained_ecapa_tdnn_model`
   - `trained_label_encoder.npy`

---

## Prediction

1. Click **"Load model and predict"**.
2. Select the `trained_ecapa_tdnn_model` directory and the `trained_label_encoder.npy` file.
3. Choose the `.mp3` file to predict its language.

---

## Features

- **ECAPA-TDNN Model**: State-of-the-art for speaker and language classification tasks.
- **Multilingual Support**: Train and classify multiple languages seamlessly.
- **Customizable Pipeline**: Easily adjust the number of files processed or the number of languages trained.

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## Contact

For any questions or feedback, please open an issue or reach out directly.
