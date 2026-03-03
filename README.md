# Predicting edestrian Crossing Intention with Behavioral and Textual Feature Fusion 
## Introduction
Predicting Crossing Intention
- **Variable pedestrian behavior**
- **Multi-modal data**
  - visual cues
  - dynamic info
  - environmental context

Importance
- Enhance road safety
- Support autonomous driving

## Dataset: JAAD 
 https://arxiv.org/abs/1609.04741  
 ### Description
- 346 short video clips
- pedestrian behaviors
- driver behaviors 
- crossing or not

## Method
### Original method in Paper 
<img width="529" height="286" alt="image" src="https://github.com/user-attachments/assets/9b860145-fe2b-4bea-a408-58410feeeb0c" />

### Our thought
- Only few features are used in the original method
- More features of the JAAD dataset can be utilized 
- Use a text encoder to encode the text features
<img width="626" height="227" alt="image" src="https://github.com/user-attachments/assets/8bb137a4-c20d-4bc5-ba77-15b01830c561" />

### The features we added
Behavior
- action
- look

Appearance
- talking on phone

Attributes
- age
- intersection
- number of lanes
- group size
- designated
- signalized
- motion direction 

## Experiment result
### Original laterfusion
<img width="383" height="222" alt="image" src="https://github.com/user-attachments/assets/f8f8149c-6f3f-4a3b-97b8-487912055797" />


### Enhanced laterfusion
#### Without text encoder
<img width="378" height="206" alt="image" src="https://github.com/user-attachments/assets/225b55f0-0f15-425d-8e34-026c7d985557" />

#### With text encoder (by using BERT)
<img width="379" height="203" alt="image" src="https://github.com/user-attachments/assets/0be49a8f-a576-46ab-9f10-1ded85f99513" />

#### With text encoder (by using DeBERTa)
<img width="376" height="207" alt="image" src="https://github.com/user-attachments/assets/7029894d-5b6e-41e1-932b-681e9f82a47d" />

### Test result
<img width="635" height="141" alt="image" src="https://github.com/user-attachments/assets/75e04b92-c16d-4454-8cf4-29845b408976" />

## Paper reference 
D. Yang et al., "Predicting Pedestrian Crossing Intention With Feature Fusion and Spatio-Temporal Attention"




