# transit-diffImage
 difference imaging for space-based transit observations

This is a fork of [stevepur/transit-diffImage](https://github.com/stevepur/transit-diffImage) at commit 2b13199, with one fix to the TESS PRF model in `transitDiffImage/tessprfmodel.py`: `tessPRF._prepare_prf` now keeps all 25 grid PRFs (the original stored only the column-2092 ones) and interpolates bilinearly between the four nearest. See the commit messages for details and checks.

To install:
clone the repository and in the top level of the repository type "pip install .".

Kepler diffimage Requires:
https://github.com/stevepur/Kepler-RaDex2Pix
