
# Beam shaping using random phase-only mask for Python.

Here is presented an iterative algorithm that locally resolves the beam shaping problem through determining high-accuracy random phase-only masks. The algorithm is based on the discrimination of the target field spatial frequencies and a relation between the intensities of the incident and target fields, which is determined from a simple physical model. Considering an extensive set of arbitrary complex input fields, particularly
those having random amplitude and phase values, the chosen variable relation between the maximal values of the intensities of the incident and target fields allows the user to find random phase-only masks with adjustable accuracy. 

The replication of these presented results also were carried out by the open source scripts in MATLAB code, available in
https://github.com/grupolatof/phase-retrieval-algorithm. [offered July 2019]


* **Authors**: [M. Yommi](https://github.com/maxiyommi), [A. Bianchetti](https://github.com/abianchetti), [P. Etchepareborda](https://github.com/PablitoE) and [A. Federico](https://github.com/alefederico).
* **Email**: grupolatof@gmail.com
* **Homepage**: http://www.inti.gov.ar

## Reference

Please use the following citation when citing phase-retrieval-algorithm in your research work:

@article{Yommi2019,
  title={Determining high-accuracy random phase-only masks for local complex modulation of light fields},
  author={M. Yommi, A. Bianchetti, P. Etchepareborda, A. Federico},
  year={2019}
}
Visit the repository with the optical description and mathematical procedures of this work in
https://www.researchgate.net/publication/337211653_Determining_high-accuracy_random_phase-only_masks_for_complex_local_modulation_of_arbitrary_light_fields


See licensing terms for details.

## Contents of the BeamFormingPyProject package
| Script  | Description |
|---|---| source
|       [main](/source/main.py) | Main script. |
|       [aux_tools](/source/aux_tools.py) | auxiliar tools script with the functions: |
|           [define_T] | Initial conditions settings. |
|           [FFT2]  | Fast Fourier Transform balanced. |
|           [iFFT2] | Inverse Fast Fourier Transform balanced. |
|           [PR] | Phase retrieval algorithm.  |
|           [speckle_gen] |  Speckle field generator. |
|           [mat2level] | Converts the matrix I to the intensity array F with values in the range [0,1]. |
|---|---| env
|       [Ei_amplitude.csv] | Intensity Data of the Input field
|       [Ei_phase.csv] | Phase Data of the Input field
|       [phi_mask.csv] | Calculated random phase-only mask
|---|---| img
|       [baboon.tif] | Phase field. Target
|       [peppers.tif] | Amplitude field. Target


For a detailed description of arguments and outputs consult the docstring in the files.
 
If you have suggestions, bugs or feature requests or want to contribute code, please email us.

## Disclaimer
All functions in this toolbox were implemented with care and tested on the examples presented in *Determining high-accuracy random phase-only masks for local complex modulation of light fields.* were possible. 
Nevertheless, they may contain errors or bugs, which may affect the outcome of your analysis. 
We do not take responsibility for any harm coming from using this toolbox, neither if it is caused by errors in the software nor if it is caused by its improper application. Please email us any bugs you find.

> Distributed under Open Source Script.




