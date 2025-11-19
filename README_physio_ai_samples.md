
# AI-Enabled Single-Channel Physiological Recorder — Sample Outputs

This folder contains sample output files that mimic the results of running an
AI/ML pipeline on three public single-channel physiological datasets:
ECG (MIT-BIH Arrhythmia), EMG (NinaPro / UCI EMG), and EEG (EEG Eye State).

## Files

1. `ecg_results_sample.csv`
   - Per-window ECG arrhythmia classification results.
   - Columns:
     - `window_id`: index of the beat/window
     - `feat_mean`, `feat_std`, `feat_ptp`: simple statistical features
     - `true_label`: ground-truth class (`normal`, `arrhythmia`)
     - `pred_label`: predicted class by the ML model
     - `modality`: always `ECG`

2. `emg_results_sample.csv`
   - Per-window EMG gesture / muscle activity classification.
   - Similar columns as ECG, with labels like `gesture_A`, `gesture_B`, `gesture_C`.

3. `eeg_results_sample.csv`
   - Per-window EEG alertness/drowsiness classification.
   - Labels: `alert`, `drowsy`.

4. `physio_ai_metrics_summary.csv`
   - High-level metrics for each modality (ECG, EMG, EEG):
     - `modality`, `task`, `accuracy`, `precision`, `recall`, `f1_score`.

5. `ecg_confusion_matrix_sample.csv`
   - Confusion matrix for ECG arrhythmia detection (normal vs arrhythmia).

6. `emg_confusion_matrix_sample.csv`
   - Confusion matrix for EMG 3-class gesture classification.

7. `eeg_confusion_matrix_sample.csv`
   - Confusion matrix for EEG drowsiness detection (alert vs drowsy).

## Usage

- Include these CSVs as sample outputs in your project submission or GitHub repo.
- Use them to generate tables and plots (e.g., confusion matrix heatmaps).
- They align with the project description: AI-Enabled Single-Channel Physiological Recorder
  with ECG, EMG, and EEG support.

Note: Values are synthetic but structured to resemble realistic model outputs and metrics.
