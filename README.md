
# .github

The [Eclipse core EDC](https://github.com/eclipse-edc/Connector) uses the [Eclipse .github actions](https://github.com/eclipse-edc/Connector).

However, they used `@main` as a version, which was doing its job at the time that any version was initially used, but those older script are now replaced by newer script versions. This causes problems when the new scripts are not compatible with the former code or build setup.

We needed to both:
* pin down the older scripts that were used during the build of the `core-edc` fork
* update those scripts as they became obsolete (obsolete dependencies), keeping their behaviour.

This fork of the `Eclipse .github` repository aims at doing exactly this.

The tags named after the forked branch in the `core-edc` e.g `0.7.2.A` track the versions that are in use with the `core-edc` fork `sovity/0.7.2.x`.

The `core-edc` fork version and this repo's version don't need to be in sync or the same in the entire build file. These are just workaround to keep the build working.
