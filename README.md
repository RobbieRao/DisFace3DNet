# DisFace3DNet

**Interpretable Facial Attractiveness Prediction via 3D Component Disentanglement**

> **Status: Coming soon.** This repository accompanies a manuscript currently under review. The implementation and the processed component-data package used in the paper will be released upon acceptance, subject to the terms of the original datasets and external model providers.

DisFace3DNet constructs an aggregate facial-attractiveness estimate from seven explicit component outputs: identity-derived shape, skin, hair, light, background, expression, and pose. Each output participates directly in score assembly.

## Method at a glance

**Component Disentanglement** → **Dynamic Component Encoder / Static Component Encoder** → **Component Score Fusion**

The component-specific branches produce five nonnegative static scores and two signed dynamic responses. Global fusion coefficients are learned during training and fixed at inference, making the weighted component contributions available with the final rating.

## Planned release

- training and inference code;
- component-input preprocessing and reconstruction scripts;
- processed component representations, annotations, split manifests, and evaluation metadata used in the paper, where redistribution is permitted;
- scripts for reproducing the reported tables and figures;
- pretrained checkpoints, where redistribution is permitted;
- instructions for regenerating restricted processed artifacts from officially obtained source datasets.

## Data availability

The processed package will be released as completely as the original dataset licenses, participant-privacy requirements, and provider policies permit. Original SCUT-FBP5500, SCUT-FBP500, and LiveBeauty face images will not be mirrored when their terms prohibit redistribution. In those cases, this repository will provide manifests and deterministic preprocessing scripts so authorized users can regenerate the component inputs from official dataset copies.

## Citation

Citation metadata will be updated when the paper is accepted. A provisional record is available in [`CITATION.cff`](CITATION.cff).

## License

Code, model weights, and derived data may require different terms. Their applicable licenses will be published with the release.
