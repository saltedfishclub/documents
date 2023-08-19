以 [中文版本](./Evolution.md) 为主。

# Version Evolution

SaltedFish Club continuously maintains all declared *unarchived* APIs/libraries/programs to introduce new features, improve APIs, etc. 
Maintainers rigorously drive each modification and provide a migration period. 

**In the absence of project documentation describing the update strategy change, this serves as the baseline**.

# Semantic Versioning

We follow the [Semantic Versioning 2.0](https://semver.org/) specification for naming.

During development, Maintainers release milestone versions with suffixes like `-M1`, `-M2`, etc. These versions mark the completion of a series of functionalities, and within milestone versions, new API changes may be introduced, making them unstable.
Before the major version is released, Maintainers publish final preview versions with the `-RC` version suffix, indicating that the new version's API has been finalized, with only minor internal optimizations or bug fixes remaining before the stable release.

# Update Compatibility

For the `x.y.z` version number:

- When `z` increases, only bug fixes and necessary code additions are made, with no breaking changes.
- When `y` increases, there will always be API changes (introduction/deprecation). Deprecated APIs will be removed after two minor versions to ensure backward compatibility. For changes with more significant disruptive updates, Maintainers always allocate additional maintenance time for the y version, but the period is one-sixth of the normal LTS (Two months).
- When `x` increases, any API can change, with no backward compatibility guarantee. An LTS (Long Term Support) version is released every two `x` versions.
    - For an LTS version of `x`, it is always based on the last `y.z` version under `x`, meaning that other `y.z` versions under `x` will always become invalid.

# Deprecation

Deprecated APIs are always marked with the `@Deprecated` annotation, and developers receive warnings at runtime/compile time.
As APIs/runtime libraries always add more features and support, we strive to ensure smooth migration while maintaining long-term support versions.
Usually, the support time for a long-term support version (LTS) is one year, while for a y version's "LTS," it is one month. LTS versions *do not receive any feature updates*, only bug fixes are provided.
