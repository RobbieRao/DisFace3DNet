# DisFace3DNet

**Explainable Facial Attractiveness Prediction via 3D Component Disentanglement**

> **Status: Coming soon.** This is the project page for the accompanying paper. Upon acceptance, we plan to release the implementation, permitted processed component data, scripts to regenerate restricted artifacts, and trained weights where redistribution is allowed by the original datasets and external model providers.

DisFace3DNet constructs an aggregate facial-attractiveness estimate from seven explicit component outputs: identity-derived shape, skin, hair, light, background, expression, and pose. Each output participates directly in score assembly.

## Method at a glance

**Component Disentanglement** → **Dynamic Component Encoder / Static Component Encoder** → **Component Score Fusion**

The component-specific branches produce five nonnegative static scores and two signed dynamic scores. After joint training, the network is frozen and fusion coefficients are fitted on its standardized outputs. The resulting overall prediction has seven additive component terms and an intercept.

## Planned release

- training and inference code;
- component-input preprocessing and reconstruction scripts;
- processed component representations, annotations, split manifests, and evaluation metadata used in the paper, where redistribution is permitted;
- scripts for reproducing the reported tables and figures;
- pretrained checkpoints, where redistribution is permitted;
- instructions for regenerating restricted processed artifacts from officially obtained source datasets.

## Data availability

The paper evaluates SCUT-FBP5500. Processed component data will be shared where the original dataset terms, participant-privacy requirements, and provider policies permit. Original face images will not be mirrored where redistribution is prohibited. For restricted processed artifacts, we plan to provide manifests and regeneration scripts for use with officially obtained dataset copies.

## Citation

Citation metadata will be updated when the paper is accepted. A provisional record is available in [`CITATION.cff`](CITATION.cff).

## License

Code, model weights, and derived data may require different terms. Their applicable licenses will be published with the release.
