# Plant Disease Classifier

A MobileNetV2 implementation built with transfer learning in TensorFlow for Plant Disease classification.

## Concepts Implemented

- Transfer Learning (ImageNet pretrained MobileNetV2)
- Prefetching
- Eraly Stopping
- Model Checkpointing
- Preprocessing
- Data Augmentation

## Dataset

- PlantVillage
- 15 classes
- 224x224 RGB images

## Results

| Experiment | Val Accuracy |
|------------|---------------|
| Baseline | 92.6% |
| +  |  |

## Experiment 1: Frozen Base Model

- MobileNetV2 pretrained on ImageNet
- Base model frozen
- Epochs: 10
- Validation Accuracy: 92.6%

## Future Improvements

- Fine-tune upper MobileNetV2 layers
- Compare frozen vs fine-tuned performance
- Add confusion matrix analysis
- Save and evaluate best model
  
## Project Status

✅ In Progress
