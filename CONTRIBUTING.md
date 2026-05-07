# Contribution Guidelines

Being an open-source project, we encourage the community to submit patches and issues
directly to the project.
This project is made to be collaborative, and we appreciate the usage of standards and
collaborative methods for submissions.

## To begin with:

* For each project component you aim to contribute to, please check the component specific CONTRIBUTING.md file if it exists. Othewise, this very file is applicable.

* Issues, features and security tracking is done with Github issues, pull-requests and security reports.
  Milestones are used in order to define a clearer roadmap.

* A Continuous Integration (CI) system runs on every Pull Request (PR). All repositories use this contribution model. It requires at least one maintainer's positive review before being merged.

## Contribution buidelines

The following guidelines must be respected by all contributors:

* When contributing, please use the ususal fork+pull-request Github model.
* When publishing a bug through issues, please specify properly the use case and a way de reproduce.

* When proposing a feature, be sure to properly define the usage.

* PRs should target the `main` branch, backports to LTS is under the maintainer's control when these branches exists.

* If a contribution requires a large amount of code, please decompose in multiple consecutive pull-requests, to make PR review easier.

* All pull-request will be checked for non-regression and are validated on real hardware.

* All modified file must have the SPDX header copyright line updated with the PR author. All new file must have a proper SPDX header (checked by CI).

* Please avoid adding new external dependencies. Dependabot is used for dependency analysis but their number should stay small enough.

* When publishing a vulnerability fix, the PR title **must** start with `cve:` tag and be dedicated to CVE fix. Vulnerabilities are created and published using Github GHSA and stored in the Outpost-OS advisories repository.
