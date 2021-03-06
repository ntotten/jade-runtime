# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## 2.0.0
### Changed
- `classes()` has been optimized, making it more than 9x faster.
- `style()` has been optimized, making it 3-9x faster in average cases.
- `escape()` has been optimized again, now with another 1-4x boost from the
  last release.
- `attrs()`, `attr()`, and `merge()` also got some minor improvements.
  Although not benchmarked, we expect the new versions to perform better than
  last release.

### Deprecated
- Internal variables, or variables or functions that were not exported but
  visible through `require('jade-runtime/build')`, will not be visible through
  `require('jade-runtime/build')` anymore.
- `jade_encode_html_rules` and `jade_encode_char`, two internal variables, have
  now been removed. Please note that any further changes to these internal
  variables will not come with a major bump.

## 1.1.0 - 2015-07-09
### Changed
- `escape()` has been optimized, making it about 20-30% faster. The new
  implementation is inspired by the one from EJS.

## 1.0.0 - 2014-12-28
### Added
- Initial release
