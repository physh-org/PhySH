# PhySH Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2018-06-13
### Added
- Initial release

## [1.1.0] - 2018-08-02
- Significant updates in the Fluid Dynamics section, including adding a few new concepts, moving all the fluid flow types that had been under "Fluid flows" to be more directly under "Fluid Dynamics Research Areas", and cleaning up some overly detailed terms.

## [1.1.1] - 2018-09-07
- Fix lowercase label that should have been uppercase

## [2.2.0] - 2021-12-22
- Identifier normalization: standardizes all PhySH identifiers to use the full UUID format with hyphen characters. A new file, uuid_mapping.csv, is included which shows the pairing of old and new identifier values where they have been changed.
- delete identifiers that had been deprecated in previous releases. The file 'deprecated.csv' lists those old identifiers that have now been removed, and suggested replacement id's if any.
- combined mapping file, 'full_mapping_2.0.csv' is also included, which combines both the uuid mapping and the deprecated concept mapping.
- New concepts added for quantum information
- New concepts and discipline added for energy science
- Some additional concepts added in condensed matter
