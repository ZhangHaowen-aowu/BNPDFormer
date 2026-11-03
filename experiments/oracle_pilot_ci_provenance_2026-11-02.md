# Oracle pilot interval table provenance

- Manuscript table: `experiments/tables/oracle_pilot_ci.tex`, label `tab:oracle-pilot-ci`.
- Point-estimate source located in `D:/Capstone/isaac_factory/瓶颈groundtruth有效性实验.md`, current Pilot results, Ops row; manuscript snapshot: `experiments/data/label_validity_dev_tyx_8767583.json`. These record only rounded estimates (0.531/0.556/0.685/0.716/0.722).
- More precise percentage estimates and all interval endpoints were supplied by the author in the 2026-11-02 chat. They agree with the rounded source values. Widths were checked as upper minus lower; percentage widths are in percentage points.
- Searches including ignored files in both `D:/Capstone/isaac_factory` and `_isaac_factory` located no per-anchor oracle JSON/CSV exports or saved interval summaries. These intervals have therefore not been independently recomputed.
- Current `factory_bn/eval_label_validity.py` implements episode means followed by percentile bootstrap (`mean_ci`, 2,000 resamples; metric-specific CRC32 seed). Without the original run outputs, this does not establish that the supplied intervals used this procedure. The manuscript consequently does not attribute an unverified interval estimator.
- The report describes three disturbance-free episodes and claims nine anchors per episode, whereas the existing evidence snapshot flags an anchor-count discrepancy with launcher defaults. No anchor count is asserted in the added table.
- No new simulation, significance test, or cross-condition inference is implied by this addition.
