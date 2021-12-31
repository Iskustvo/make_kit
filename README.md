# Make Kit
Generic build system for modern C++ projects.

## Current goals

* Build simple C++ library for Linux.
  * Be able to build static and dynamic versions of the library.
  * Be able to build library in debug and release mode.
  * Nested subprojects/modules are NOT supported.
* Support tests.
  * Unit tests without mocking.
  * Unit tests with mocking.
* Generic detection of source files.
  * Build system should automatically include all *.cpp and *.hpp files in configured directories and subdirectories.
  * Developer doesn't need to modify the build system configuration after adding/removing a header/source/test file.
* Automatic dependency tracking for all files.
  * Build system will track dependencies and only rebuild/retest files that are outdated.
* Support incremental testing.
  * Optionally track dependencies between classes and test a class only after its depedency classes have passed the tests.
* Generate code documentation.
* Generate code coverage.
