# Plant Disease Classifier

A MobileNetV2 implementation built with transfer learning in TensorFlow for Plant Disease classification.

## Concepts Implemented

* Transfer Learning (ImageNet pretrained MobileNetV2)
* Prefetching
* Early Stopping
* Model Checkpointing
* Preprocessing
* Data Augmentation

## Dataset

* PlantVillage
* 15 classes
* 224x224 RGB images

## Results

|Experiment|Val Accuracy|
|-|-|
|Frozen Base Model|92.6%|
|Fine-Tuned Model|95%|

## Experiment 1: Frozen Base Model

* MobileNetV2 pretrained on ImageNet
* Base model frozen
* Epochs: 10
* Validation Accuracy: 92.6%

## Experiment 2: Fine Tuned Model

* Fine-Tuned MobileNetV2 model on PLantVillage dataset
* Upper 20 layers(includes last 2 bottleneck blocks) fine tuned
* Epochs: 10
* Validation Accuracy: 95%

## Key Findings

- Transfer learning dramatically outperformed training from scratch.
- Fine-tuning only the upper layers improved validation accuracy from 92.6% to 95.0%.
- MobileNetV2 pretrained on ImageNet transferred effectively to plant disease classification.

## Evaluation

- Validation Accuracy: 95.0%
- Confusion Matrix Analysis
  <img width="487" height="460" alt="Screenshot 2026-06-20 194315" src="https://github.com/user-attachments/assets/efe6e622-31f4-4335-8a10-20f66f2cb10c" />

- Classification Report
  <img width="461" height="272" alt="Screenshot 2026-06-20 194029" src="https://github.com/user-attachments/assets/33ff126a-6fa4-4b1e-b3f4-de5ba495cc00" />


## Future Improvements

* Fine-tune upper MobileNetV2 layers✅
* Compare frozen vs fine-tuned performance✅
* Add confusion matrix analysis✅
* Save and evaluate best model✅

## Project Status

✅ Completed

