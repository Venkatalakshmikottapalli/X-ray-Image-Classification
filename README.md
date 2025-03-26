# X-ray-Image-Classification
Canine cardiomegaly, characterized by heart enlargement,
presents significant diagnostic challenges in veterinary
medicine. This research introduces a Deep Convolutional
Neural Network (Deep CNN) architecture designed
for the automated detection of cardiomegaly in canine radiographs.
Unlike traditional methods that rely on pretrained
models such as VGG16 and EfficientNetB7, the proposed
Deep CNN offers a fully independent, end-to-end solution,
removing the need for transfer learning. Tailored
specifically for canine cardiac imaging, the architecture
demonstrates robust feature extraction capabilities. Experimental
results show that the approach achieves comparable
or superior accuracy to existing techniques while significantly
reducing computational complexity. This study
presents a streamlined yet highly effective model utilizing
Deep CNNs to efficiently process extracted features. Comparative
evaluations with VGG16 and EfficientNetB7 highlight
the improved performance and efficiency of the proposed
method. The findings underscore the potential of integrating
Deep CNN based architectures into veterinary diagnostics,
contributing to enhancing automated cardiac assessment
tools in clinical practice.

##  Dataset Description
The DogHeart dataset consists of 2,000 high-resolution canine
thoracic radiographs collected from Shanghai Aichong
Pet Hospital[4]. To ensure privacy, all images were cropped
to remove identifiable information. The dataset is categorized
into three classes based on the Vertebral Heart Score
(VHS): small hearts (< 8.2), normal hearts (8.2–10), and
large hearts (> 10). While the normal and large heart categories
are well-represented, the small heart category has
fewer samples.
## Model Architecture
The proposed architecture, DeepCNN, integrates convolutional
neural networks (CNN) for feature extraction with
fully connected layers for classification. This design effectively
captures spatial patterns within the canine thoracic
radiographs, followed by the classification of the extracted
features into distinct heart size categories.
The CNN layers are responsible for extracting high-level
spatial features from the input images. These layers include
multiple convolutional operations, each followed by
batch normalization and ReLU activation to model complex
patterns. Max-pooling layers are used after each convolutional
block to reduce spatial dimensions, improving computational
efficiency while retaining important features. To
mitigate overfitting and enhance generalization, a dropout
layer with a rate of 0.5 is applied after the fully connected
layers.
The fully connected layers perform the final classification
based on the extracted features. The network includes
three fully connected layers, with ReLU activations applied
after the first two layers. The final layer produces the class
scores for three heart size categories using a linear activation
function.
The architecture’s innovative approach addresses the
critical challenge of automated cardiac size assessment in
veterinary diagnostics by leveraging advanced deep learning
techniques. By integrating sophisticated feature extraction
mechanisms with precise classification strategies,
DeepCNN demonstrates significant potential for objective
and consistent medical image analysis.

<img width="415" alt="image" src="https://github.com/user-attachments/assets/71a4a55d-361e-4a54-baf0-b95ea30e8989" />

