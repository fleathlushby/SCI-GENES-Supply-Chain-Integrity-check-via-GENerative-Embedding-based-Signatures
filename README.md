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

<p align="center">
  <img src="https://github.com/fleathlushby/SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures/blob/main/puf_components.png" width="500"/>
</p>
<p align="center">
  <em><b>Figure 2:</b>This is a global view of the different components in the PUF structure, which includes the following: (a) PUF IC, (b) Shift Registers, (c)Switches, (d) 4-bit Adder. All of the images are captured using our in-house scanning electron microscope (SEM) at different magnification ranges.</em>
</p>

<p align="center">
  <img src="https://github.com/fleathlushby/SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures/blob/main/gdsii_puf_equivalence.png" width="500"/>
</p>
<p align="center">
  <em><b>Figure 3:</b>Components identification using GDSII matching. A portion of the M1 layer switch chain 
(a) SEM image, (b) GDSII file image.</em>
</p>

<p align="center">
  <img src="https://github.com/fleathlushby/SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures/blob/main/segmentation_metal_via.png" width="500"/>
</p>
<p align="center">
  <em><b>Figure 4:</b> Metal and Via segmentation from SEM images. (a) SEM Image of M4 Layer of ATMEGA 328P IC, (b) Metal Trace Mask,
(c) Via Mask, (d) GAN Generated Overlaid Mask.</em>
</p>

<p align="center">
  <img src="https://github.com/fleathlushby/SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures/blob/main/pcb_counterfeit.png" width="500"/>
</p>
<p align="center">
  <em><b>Figure 5:</b> PCB counterfeit detection using X-Ray Microscope (XRM). The differences between XRM images of original (row 1) and duplicate (row 2) Arduino UNO PCBs.</em>
</p>

<p align="center">
  <img src="https://github.com/fleathlushby/SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures/blob/main/different_fingerprints.png" width="500"/>
</p>
<p align="center"><em><b>Figure 6:</b> XRM images of three different classes of PCBs : (a) Arduino UNO, (b) Raspberry Pi, and (c) STM32F407G Discovery Kit. Three different boards in each class exhibit unique variation in metal and solder deposition. We consider these anomalies as the unique fingerprints for each board.</em></p>

<p align="center">
  <img src="https://github.com/fleathlushby/SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures/blob/main/IMG_20250327_132459.jpg" width="500"/>
</p>
<p align="center"><em><b>Figure 7:</b> Our in-house Focused Ion Beam (FIB) and Scanning Electron Microscope (SEM) facility.</em></p>

<p align="center">
  <img src="https://github.com/fleathlushby/SCI-GENES-Supply-Chain-Integrity-check-via-GENerative-Embedding-based-Signatures/blob/main/IMG_20250327_132520.jpg" width="500"/>
</p>
<p align="center"><em><b>Figure 8:</b> Our in-house X-Ray Microscope facility.</em></p>
