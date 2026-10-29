# NILS model files

The trained model files NILS reads as model inputs, for sites that run its post-contrast and body-part pipelines. Downloading or using them means accepting `LICENSE.md` (research and evaluation use only, no clinical decisions, no redistribution).

Each folder holds one model's file; `cards/` holds each model's card as NILS registered it; `SHA256SUMS` has every file's digest, which is the digest the card names.

| Model | File | Read by |
|---|---|---|
| postcontrast-student@pc-student3 | student.safetensors | postcontrast-cascade |
| postcontrast-fusion@r1 | fusion.json | postcontrast-cascade, postcontrast-full |
| postcontrast-arms@r1 | arms.json | postcontrast-full |
| postcontrast-cascade@c1-fs3-m | cascade.json | postcontrast-cascade, postcontrast-full |
| bodypart-tiny@r7, bodypart-fusion@r7, bodypart-fusion-coarse@r7, bodypart-student@s1-r7, bodypart-defer@d3-r7, bodypart-cascade@r7-fast | as listed | bodypart-infer-fusion |

Register each at your site with its card and its file, then keep the file where runs find it:

```sh
nils model register --card cards/postcontrast-fusion-r1.card.json --artifact postcontrast-fusion-r1/fusion.json
nils model keep postcontrast-fusion@r1 --artifact postcontrast-fusion-r1/fusion.json
```

The post-contrast fusion answers only at the sites it was calibrated for; every other site gets "not sure" until it fits its own pair (`nils-postcontrast calibrate`, since 0.3.0). The cards were written when these were site models kept at one site; the line in each card's limits saying so predates their publication under this licence.

Citation: Chamyani N, et al. NILS model files. Kineuro, Karolinska Institutet, 2026. https://github.com/kineuro/nils-models
