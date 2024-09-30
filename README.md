## Adversarial Attacks: 
These are subtle, often imperceptible, perturbations added to images that fool deep learning models into making incorrect predictions. Examples of popular attacks include FGSM (Fast Gradient Sign Method), PGD (Projected Gradient Descent), and DeepFool.
## Objective: 
To explore novel defenses against these attacks or improve upon existing defense mechanisms such as adversarial training, robust optimization, or using auxiliary models for detection.
Currently trying out FGSM and PGD on a normally trained ResNet-18 pretrained model. Normally trained models are models trained on a cleaned dataset where adversarial examples aren't introduced yet.

## Research Question: 
How can we improve the robustness of deep learning models in image classification tasks to adversarial attacks without sacrificing accuracy?
