# Attacking CNN Models and Testing Their Robustness
## Adversarial Attacks: 
These are subtle, often imperceptible, perturbations added to images that fool deep learning models into making incorrect predictions. Examples of popular attacks include FGSM (Fast Gradient Sign Method), PGD (Projected Gradient Descent), and DeepFool.
## Objective: 
To explore novel defenses against these attacks or improve upon existing defense mechanisms such as adversarial training, robust optimization, or using auxiliary models for detection.

## Research Question: 
How can we improve the robustness of deep learning models in image classification tasks to adversarial attacks without sacrificing accuracy?

At the moment, I and exploring whether robustness can be transfered from one set of attack to the others.
First, I will take a pretrained standard or normal CNN architecture (ResNet-18 atm) and fine-tune it on the CIFAR 10 dataset (will later apply it to high resolution images).
Then, test it on the standard or normal fine-tuned model and also on adversarial examples (also called adversarial attacks).
I will start with the simplest to compute and relatively cheaper attack - FGSM.
Then, I will adversarially train the standard model on the FGSM attacks and evaluate this adversarial-trained model on other harder adversarial attacks like the PGD and the CW attacks.

After this, I would start from scratch again but attacking the standard or normal fine-tuned model with the CW attack (understood that models trained on these kinds of attacks are relatively more robust compared to the others; I will find out :))
Then, reverse the order to see the influence. Boyy, this is going to be a fun ride.
