# xAPI assessment profile

This documentation intends to describe assessment profile defined by the Gaia-X organisation.

## Statements

### Participation

These statements are required to know which assignment has been proposed to learners, when it was available, who answer the assignment and what are the individual results for each participant. This specification complies to the cmi5 specification.

All these statements are **MANDATORY** in order to comply with this profile.

- [Launched](./statements/mandatory/launched.md)
- [Initialized](./statements/mandatory/initialized.md)
- [Completed](./statements/mandatory/completed.md)
- [Passed](./statements/mandatory/passed.md)
- [Failed](./statements/mandatory/failed.md)
- [Terminated](./statements/mandatory/terminated.md)

:warning: In some assessment tools, the implementation does not allow to track contextual information about the assessment itself.
Following statements, ONLY WHEN it is technically not possible to be tracked are optional:
- launched
- initialized
- completed
- terminated

### Main interactions

These statements are helpful to get to know what happened in detail during the assessment. In an analytics perspective, it gives information on how student behave to fulfill (or aband) the assessment and give pedagogical feedback about it to improve the assessment.

All these statements are **HIGHLY RECOMMENDED**.

- [Shew answer](/statements/optional/shew-answer.md)
- 

### Other interactions

These statements give more details on learners during an assessment.

All these statements are **OPTIONAL**.

## Contributors

| Github user  | Name            | Company/Institution         |
|----------------|-----------------|-----------------------------|
| [@quitterie-lcs](https://github.com/quitterie-lcs) | Quitterie Lucas | [France Université Numérique](https://www.france-universite-numerique.fr/en/) |

