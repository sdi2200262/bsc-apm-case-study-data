# BSc APM Case Study Data

Encrypted research data for the BSc thesis case study comparing Agentic Project
Management with GitHub Spec-kit for AI-assisted software development.

## Encryption and reproducibility

`dataset.enc` contains the complete dataset as one authenticated encrypted
archive. Authentication makes an incorrect secret or a modified archive fail
explicitly instead of producing corrupted plaintext.

The secret required for decryption is kept outside this repository and may be provided
privately to authorised reviewers. A reviewer with the secret can recover the dataset,
verify the archive's integrity, and reproduce the reported analysis.

## Contents

The decrypted archive holds one directory per session under
`submissions/<pid>/<session>_<framework>_<model>/`, with the session transcript archive, the
parser outputs (`parser_data.json`, `parser_metrics.json`), and the grader outputs
(`grader_results.json`, `grader_results_compact_serialization.json`). The questionnaire
responses are under `questionnaire/`. The thesis README describes the analysis config that
points at these files.

## Licence and access

This repository is not openly licensed, as it holds personal data about human participants,
protected by encryption.

- `dataset.enc` may be copied and redistributed unmodified, with the [LICENSE](LICENSE).
- The secret required for decryption stays with the author. Independent reviewers receive it once they
  agree in writing to use the data only to verify the reported analysis, make no attempt to identify
  participants, share neither the decrypted data nor the secret, and delete both once verification
  is done. Any work that draws on the data credits the thesis as its source by citing it.

To request access, write to haidemenoss@gmail.com or sdi2200262@di.uoa.gr with your role and purpose.

## Related repositories

- [bsc-apm-case-study-infra](https://github.com/sdi2200262/bsc-apm-case-study-infra): the parser and grader used to produce the dataset artefacts.
- [bsc-apm-case-study-task](https://github.com/sdi2200262/bsc-apm-case-study-task): the task and participant package.
- [bsc-apm-thesis](https://github.com/sdi2200262/bsc-apm-thesis): the thesis.
