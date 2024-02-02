# Skin Concern Identification

This repository introduces a Multimodal approach to identify diverse skin concerns by allowing users to submit skin images along with corresponding symptoms. The project explores both Early Fusion and Late Fusion techniques to improve the precision of skin concern predictions.

## Skin Concerns

### Acne-Prone Skin
Characterized by the presence of acne, including pimples, blackheads, and whiteheads. Acne-prone skin is often susceptible to inflammation and redness.

### Hyperpigmented Skin
Refers to skin with increased pigmentation, leading to dark spots or patches. Hyperpigmentation can be triggered by factors such as sun exposure, inflammation, or hormonal changes.

### Hypopigmented Skin
Involves a loss of skin pigmentation, resulting in lighter or white areas on the skin. Hypopigmentation may be associated with conditions like vitiligo or certain skin infections.

### Rosacea-Prone Skin
Characterized by persistent redness on the face, often accompanied by visible blood vessels, bumps, or pimples. Rosacea-prone skin tends to be sensitive and prone to flushing.

## Fusion Techniques Explored

- **Early Fusion:** This technique involves combining information from both image and symptom inputs at an early stage in the model architecture.

- **Late Fusion:** Merging information from image and symptom inputs occurs at a later stage in the model architecture.

## Pretrained Models Used

### CNN Models
- DenseNet121
- MobileNetV2
- VGG19
- ResNet50

### BERT Model
- bert-base-multilingual-cased (mBERT)
- XLM-RoBERTa
  

## Fusion Approaches

- DenseNet121-mBERT with Early Fusion
- DenseNet121-mBERT with Late Fusion
- DenseNet121-XLM-RoBERTa with Early Fusion
- DenseNet121-XLM-RoBERTa with Late Fusion
- MobileNetV2-mBERT Early Fusion
- MobileNetV2-mBERT Late Fusion
- VGG19-mBERT Early Fusion
- VGG19-mBERT Late Fusion
- ResNet50-mBERT Early Fusion
- ResNet50-mBERT Late Fusion
- ResNet50-XLM-RoBERTa Early Fusion
- ResNet50-XLM-RoBERTa Late Fusion

## Evaluation Metrics

| Model                        | Test Accuracy | Test Precision | Test Recall | Test F1 Score | Test Jaccard Score |
| ---------------------------- | ------------- | -------------- | ----------- | ------------- | ------------------- |
| DenseNet121-mBERT Early Fusion | 0.283         | 0.225          | 0.283       | 0.212         | 0.128               |
| DenseNet121-mBERT Late Fusion  | 0.200         | 0.192          | 0.200       | 0.165         | 0.093               |
| DenseNet121-XLM-RoBERTa Early Fusion | 0.2        | 0.190          | 0.2       | 0.145        | 0.082               |
| DenseNet121-XLM-RoBERTa Late Fusion  | 0.2         | 0.084          | 0.199       | 0.103         | 0.060               |
| MobileNetV2-mBERT Early Fusion | 0.250         | 0.247          | 0.250       | 0.232         | 0.134               |
| MobileNetV2-mBERT Late Fusion  | 0.200         | 0.235          | 0.200       | 0.183         | 0.102               |
| VGG19-mBERT Early Fusion      | 0.300         | 0.231          | 0.300       | 0.214         | 0.133               |
| VGG19-mBERT Late Fusion       | 0.283         | 0.341          | 0.283       | 0.250         | 0.146               |
| ResNet50-mBERT Early Fusion   | 0.267         | 0.156          | 0.267       | 0.175         | 0.107               |
| ResNet50-mBERT Late Fusion    | 0.383         | 0.472          | 0.383       | 0.353         | 0.222               |
| ResNet50-XLM-RoBERTa Early Fusion   | 0.216         | 0.203          | 0.216       | 0.181         | 0.103               |
| ResNet50-XLM-RoBERTa Late Fusion    | 0.3         | 0.309          | 0.3       | 0.296         | 0.174               |

