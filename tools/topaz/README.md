# Topaz Galaxy Tool Suite

This directory contains Galaxy Tool wrappers for **Topaz 0.3.20**, a pipeline for particle detection and deep denoising in cryo-electron microscopy (cryo-EM) images.

## Included Tools

1. **Topaz Preprocess**: Downsample and normalize micrographs using a 2-component Gaussian mixture model (GMM) to standardize exposure across the dataset.
2. **Topaz Train**: Train convolutional neural network (CNN) classifiers (e.g. ResNet-8, ResNet-16) from positive and unlabeled (PU) examples.
3. **Topaz Extract**: Segment micrographs with a trained model and extract particle coordinates using a non-maximum suppression (NMS) algorithm.
4. **Topaz Denoise**: Denoise micrographs and tomograms using deep U-Net architectures to enhance contrast and aid downstream particle picking.

## Requirements

The tools depend on the `topaz` package installed via Conda.

## Citations

- Bepler, T., Morin, A., Rapp, M. et al. Positive-unlabeled convolutional neural networks for particle picking in cryo-electron micrographs. *Nat Methods* 16, 1153–1160 (2019). https://doi.org/10.1038/s41592-019-0575-8
- Bepler, T., Kelley, K., Noble, A.J. et al. Topaz-Denoise: general deep denoising models for cryoEM and cryoET. *Nat Commun* 11, 5208 (2020). https://doi.org/10.1038/s41467-020-18952-1
