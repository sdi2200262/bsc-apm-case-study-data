# BSc APM Case Study Data

Encrypted research data for the BSc thesis case study comparing Agentic Project
Management with GitHub Spec-kit for AI-assisted software development.

## Encryption and reproducibility

`dataset.enc` contains the complete dataset as one authenticated encrypted
archive. Authentication makes an incorrect secret or a modified archive fail
explicitly instead of producing corrupted plaintext.

The secret is kept outside this repository and may be provided privately to
authorised reviewers. A reviewer with the secret can recover the dataset,
verify the archive's integrity, and reproduce the reported analysis.

## Related repositories

- [bsc-apm-case-study-infra](https://github.com/sdi2200262/bsc-apm-case-study-infra): the parser and grader used to produce the dataset artefacts.
- [bsc-apm-case-study-task](https://github.com/sdi2200262/bsc-apm-case-study-task): the task and participant package.
- [bsc-apm-thesis](https://github.com/sdi2200262/bsc-apm-thesis): the thesis.
