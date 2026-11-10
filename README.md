# An Audit of Evaluation and Reporting Practice on the CMU Keystroke Dynamics Benchmark

Code and coding sheet for the paper by Joseph Black (School of Technology and Innovation, Marymount University).

## Files

- `cmu_keystroke_audit.ipynb`: Jupyter notebook that produces every result in Sections 5.3 and 6 of the paper.
- `coding_sheet.xlsx`: the audit coding sheet, covering the original benchmark paper and the 12 audited studies, with the tally and the citation conflicts in Table 2.

## Data

The notebook reads `DSL-StrongPasswordData.csv`, the CMU Keystroke Dynamics Benchmark published by Killourhy and Maxion (2009). The file is not included here. Download it from the authors' page at https://www.cs.cmu.edu/~keystroke/ and place it in the same folder as the notebook.

## Running the notebook

1. Install the libraries: `pip install numpy pandas scipy scikit-learn matplotlib`
2. Open the notebook and run all cells. The one-class SVM and the protocol comparison in Section 13 take a few minutes.

The notebook writes `per_subject_results.csv` and `correlations.csv` to the same folder.

## Where each paper result comes from

| Paper | Notebook section |
| --- | --- |
| Table 3 (reproduced detectors, zero-miss rates) | 5 and 6 |
| Table 3 (global threshold) | 7 |
| Table 4 (fixed threshold from enrollment data) | 8 |
| Section 6.4 (per-user results and correlations) | 10 and 12 |
| Section 5.3 (random forest identification accuracy) | 11 |
| Table 5 (protocol comparison, setups A to D) | 13 |
| Section 6.6 (measurement resolution) | 9 |

## Reference

K. S. Killourhy and R. A. Maxion, "Comparing anomaly-detection algorithms for keystroke dynamics," in Proc. IEEE/IFIP Int. Conf. Dependable Syst. Netw. (DSN), 2009, pp. 125-134.
