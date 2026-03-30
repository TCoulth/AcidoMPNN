# AcidoMPNN
Retraining of ProteinMPNN model specifically with acid-stable structures and sequences

Trained using the [HyperMPNN](https://github.com/meilerlab/HyperMPNN) training scripts. Also used most of the same sequence selection logic (ie same clustering and quality cutoffs).

**Structure Selection**

Sequences were filtered by organism, selecting for acidophiles, and then for the prescence of a secretion tag. After clustering at 50% sequence identity, AF2 structures were gathered and filtered by quality (>70% plddt).

**Training**

21129 total sequence/structures used. 80-10-10 training-validation-test split

<img width="563" height="455" alt="image" src="https://github.com/user-attachments/assets/888d95e5-e868-4acd-b621-25b1d6e78ae1" />

<img width="567" height="455" alt="image" src="https://github.com/user-attachments/assets/48f5e6b6-7490-428a-9382-bf8a0d5f8a0f" />

**Testing Results**

Note: Has not been experimentally tested yet. Please try!

Generated sequences were folded with high confidence with AF2. Amino acid compositions are distinct from ProteinMPNN and HyperMPNN distributions. More analysis to follow

**Use**

Point [ProteinMPNN](https://github.com/dauparas/ProteinMPNN) to the acidompnn .pt file.

