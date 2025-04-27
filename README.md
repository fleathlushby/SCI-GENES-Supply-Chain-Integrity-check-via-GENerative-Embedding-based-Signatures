# SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures
This repository presents preliminary results from our initial work on PCB counterfeit detection, IC layer identification, and segmentation.
For PCB counterfeit detection, we employ convolutional neural network (CNN)-based classification, with the Inception-V3 architecture achieving a classification accuracy of 99.14%.
IC layer identification is performed using FIB technology to distinguish the seven metal layers in an in-house designed PUF IC, while component identification is carried out through GDSII equivalence checking.
Our IC layer segmentation approach utilizes a Swin-Transformer-based GAN architecture to effectively segment metal traces and vias from SEM images.

## Experimental Results

<p align="center">
  <img src="https://github.com/fleathlushby/SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures/raw/main/ic_layers.png" width="500"/>
</p>
<p align="center">
  <em><b>Figure 1:</b> Cross-sectional view of an in-house designed PUF IC with seven metal layers. We utilize Focused Ion Beam (FIB) technology to investigate the different stacked metal layers. The IC is fabricated using ST Microelectronics 65nm process technology. The image clearly displays all the distinct seven layers, marked by labels M1 through M7. The polysilicon layer, along with the diffusion region, is also visible from the image, marked by labels Poly Si and Diff, respectively. The top and bottom part of the IC represent the passivation layers and silicon substrate, respectively.</em>
</p>

