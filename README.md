# FS-Mamba: Frequency-Structure Decoupling with Mamba for Low-Light Image Restoration

## Abstract

Low-light image restoration is challenging because insufficient illumination often coexists with noise, contrast degradation, and motion-induced structural corruption. We propose **FS-Mamba**, a frequency--structure decoupled state-space network that assigns complementary restoration objectives to the encoder and decoder. The encoder employs a **Frequency-Aware Mamba Block (FAMB)**, which estimates channel-wise spectral affinity from Fourier amplitude responses and uses it to modulate illumination-sensitive features. The decoder adopts a **Structure Restoration Mamba Block (SRMB)**, which integrates directional wavelet priors with selective state-space modeling to recover edges, textures, and local structures. This asymmetric design separates frequency-oriented illumination modeling from structure-oriented reconstruction while retaining efficient long-range dependency modeling. Experiments on **LOL-Blur**, **LOL-v1**, and **LOL-v2-Synthetic** show that FS-Mamba is effective for both joint low-light deblurring and standard low-light enhancement. With only **3.86M parameters**, FS-Mamba achieves **31.96 dB / 0.912**, **24.55 dB / 0.858**, and **26.49 dB / 0.950** in PSNR/SSIM on the three datasets, respectively.

## Network Architecture

<p align="center">
  <img src="fig/net.pdf" width="95%">
</p>

<p align="center">
  <b>Figure 1.</b> Overall architecture of the proposed FS-Mamba.
</p>

## Visual Results

<p align="center">
  <img src="fig/fig1.pdf" width="95%">
</p>

<p align="center">
  <b>Figure 2.</b> Visual comparison of FS-Mamba on low-light image restoration.
</p>

<p align="center">
  <img src="fig/fig2.pdf" width="95%">
</p>

<p align="center">
  <b>Figure 3.</b> Visual comparison of FS-Mamba on low-light image restoration.
</p>
