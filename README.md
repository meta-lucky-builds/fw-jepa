# fw-jepa

FW-JEPA: fast-weight (TTT-layer) test-time adaptation for JEPA world models.

This repo starts from [LeWorldModel](https://github.com/lucas-maes/le-wm) (commit `8edfeb3`, MIT licence, see `LICENSE-LeWM` and `README-LeWM.md`) and will add:

- a shared TTT layer module (gated fast-weight MLP, truncated BPTT) inserted into the `ARPredictor` in `module.py`
- shifted-dynamics environment wrappers for meta-training and held-out evaluation
- a reward head and a JEPA-TTT (online fine-tuning + dense replay) baseline for comparison

Setup, data and the original training/planning instructions are in `README-LeWM.md`.
