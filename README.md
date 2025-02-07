
# Eclipse EDC .github files

## About

The [Eclipse core EDC](https://github.com/eclipse-edc/Connector) uses the [Eclipse .github actions](https://github.com/eclipse-edc/Connector).

However, they used `@main` as a version, which was doing its job at the time that any version was initially used, but those older script are now replaced by newer script versions. This causes problems when the new scripts are not compatible with the former code or build setup.

We needed to both:
* pin down the older scripts that were used during the build of the `core-edc` fork
* update those scripts as they became obsolete (obsolete dependencies), keeping their behaviour.

This fork of the `Eclipse EDC .github` repository aims at doing exactly this.

## "Releasing"

The forking and tagging in this repository is done during the forking of a new EDC Connector version, and is described in the `fork.md` issue of the core EDC sovity fork: https://github.com/sovity/core-edc/blob/default/.github/ISSUE_TEMPLATE/fork.md
