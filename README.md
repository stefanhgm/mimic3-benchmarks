An Evaluation of the Doctor-Interpretability of Generalized Additive Models with Interactions
=========================

Fork of [MIMIC-III Benchmarks](https://github.com/YerevaNN/mimic3-benchmarks) introduced in [Multitask learning and benchmarking with clinical time series data](https://doi.org/10.1038/s41597-019-0103-9) by Hrayr Harutyunyan et al. to generate features for an evaluation of the doctor-Interpretability of [Generalized Additive Models with Interactions](https://doi.org/10.1145/2487575.2487579).

The instructions from the original repository also apply for this fork. Please follow the build instructions. After step six, the following command was used to generate the necessary features.

    python -m mimic3models.in_hospital_mortality.logistic.main --l2 --C 0.001 --output_dir {OUTPUT DIRECTORY} --data /data/in-hospital-mortality --features mean_and_sd --period all
