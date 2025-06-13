# Changelog

## [0.1.9] – 2025-06-13

### Added

- Add new `shard_utils` library for TVM global version 10 sharding prefix length logic
- Add `shard_utils::get_shard_from_hash` function to extract shard from hash values
- Add `shard_utils::get_shard_from_address` function to extract shard from addresses
- Add `shard_utils::change_hash_shard` function to modify shard bits in address hash part
- Add `shard_utils::change_address_shard` function to modify shard bits in address hash part
- Add `shard_utils::addresses_in_same_shard` function to compare address shards
- Add `shard_utils::hashes_in_same_shard` function to compare address hash part shards
- Add `shard_utils::pack_prefixed_state_init` function for creating state init with fixed prefix scheme
- Add `shard_utils::calc_account_hash` function for optimized fixed prefix account hash calculation
- Add comprehensive test suite for shard utilities in `shard_test.fc`
- Add `extract_low_bits` fift-asm helper

## [0.1.8] – 2025-03-03

### Added

– Add new `utils::calc_account_hash`, `utils::basechain_address_from_account_hash` and `utils::basechain_address_from_code_and_data` helpers for optimized basechain address calculation
– Add `contracts.basechain_address` method for optimized basechain address calculation

## [0.1.7] - 2024-12-12

### Added

- Add `actions.fc` library for working with c5 register
- Add `get_actions`, `get_config` and `cast_to_builder` functions to `stdlib_ext`
- Add new `utils::make_c7` helper
- Add new dict functions
- Add new constants related co c7 actions
- Add more new tests

### Fixed

- Fix `math::fp::log` for negative numbers
- Removed all `method_id` modifiers
- All recursive functions rewritten to be non-recursive to save contract size after including `autoload.fc` file

### Changed

- Test suite rewritten to `@ton/sandbox` message-based approach

## [0.1.6] - 2024-11-22

### Changed

- Improve `sqrt` function

## [0.1.5] - 2024-10-10

### Added

- Add modifier methods to `message` library.

## [0.1.4] - 2024-09-10

### Added

- Add new `utils::merge_dict` helpers.

## [0.1.3] - 2024-09-04

### Changed

- Fix `math::int::sqrt` function to handle negative numbers.

## [0.1.2] - 2024-08-23

### Added

- Add new `message` library

## [0.1.1] - 2024-06-24

### Added

- Add new address's related functions
- Add new opcodes
  
## [0.1.0] - 2024-05-02

### Added

- Add new opcodes

### Changed

- Code cleanup
- Functions that were marked as `inline_ref`, now are marked as `inline`

## [0.0.15] - 2024-04-03

### Added

- Add new primitive wrappers

## [0.0.14] - 2024-03-14

### Added

- Add new primitive wrappers
- Add new dict functions

## [0.0.13] - 2024-01-18

### Added

- Add new hash functions
- Add new message modes & modifiers
- Add new c7 opcode wrappers

### Changed  

- `Console::log` doesnt require explicit to tuple conversion

## [0.0.12] - 2023-12-13

### Added

- Add `math::fp::complement` math function 
- Add `console::pretty_coins`, `console::pretty_coins`, `console::log` functions
- Add `change_lib` and `set_lib` to `stdlib_ext`
- Add `address::check_workchain_nofail` and `address::is_hole` to address lib
- Add `ctx::init_wempty` to ctx lib

### Changed  

- Change math libs structure
- Change `math::int::pow_dec` to `math::fp::pow_dec`
- Change capitalize public constants

### Fixed

- Fix use `muldiv` where needed

## [0.0.11] - 2023-11-17

### Added

- Add `interfaces` lib: helper for `jetton` and `any` messages with builder support
- Add `HOLE_ADDRESS` constant
- Add new `msgs` lib helpers that accept builder, prefixed by `msgs::send_b*`
- Add new math functions

### Changed

- Refactor `math` lib into two separate libs

## [0.0.10] - 2023-11-02

### Added

- Add new `math` functions: `pow`, `ln`, `exp` and `log` 
- Add new `address` functions: `check_workchain` and `check_hashpart`
- Add SBT NFT missing opcodes
- Add additional wrapper for unsupported opcodes

## [0.0.9] - 2023-10-12

### Added

- Add `time` library (constants helpers and utilities)
- Add constants values for max uint
- Add status load/store functions
- Add reserves library

## [0.0.8] - 2023-08-08

### Added

- Add `begin_message` util 

### Fixed

- Fix tests not throwing on errors

## [0.0.7] - 2023-07-20

### Added

- Add `op::excesses` opcode
- Add `load_query_id & store_query_id` helpers functions
- Add `load_opcode & store_opcode` helpers functions
- Add dict helper library
- Add `address.is_none()` helper
- Add `cell.is_empty()` helper
- Add dump utils library
- Add `utils.number_to_slice`
- Add math library
- Add cell utils library
- Add test util `assert` library
- Add tests

### Changed

- Rename library `address_utils` to `address`

## [0.0.6] - 2023-06-23

### Added

- Add `load_time & store_time` helpers functions (alias `load_uint(64) & store_uint(64)`)
- Add `load_uint* & store_uint*` helpers functions to work with fixed uints (8, 16, 32, 64, 128, 256)
- Add quiete messages send modes (prefixed with `Q`)
- Add `equal_cell` function

## [0.0.5] - 2023-06-19

### Fixed

- Add missing skip bits on bounced calls

## [0.0.4] - 2023-05-31

### Added

- Add `address_utils` library
- Add standard opcodes (NFTs & FTs)
- Add `as_slice` helper function

### Removed

- Remove `address` library

## [0.0.3] - 2023-05-30

### Changed

- Cosmetic changes
- Rename `contex` lib to `ctx`

## [0.0.2] - 2023-05-29

### Added

- Add `address` library

## [0.0.1] - 2023-05-26

### Added

- Add initial library release

[0.1.8]: https://github.com/ston-fi/funcbox/tree/v0.1.8
[0.1.7]: https://github.com/ston-fi/funcbox/tree/v0.1.7
[0.1.0]: https://github.com/ston-fi/funcbox/tree/v0.1.0
[0.0.15]: https://github.com/ston-fi/funcbox/tree/v0.0.15
[0.0.14]: https://github.com/ston-fi/funcbox/tree/v0.0.14
[0.0.13]: https://github.com/ston-fi/funcbox/tree/v0.0.13
[0.0.12]: https://github.com/ston-fi/funcbox/tree/v0.0.12
[0.0.11]: https://github.com/ston-fi/funcbox/tree/v0.0.11
[0.0.10]: https://github.com/ston-fi/funcbox/tree/v0.0.10
[0.0.9]: https://github.com/ston-fi/funcbox/tree/v0.0.9
[0.0.8]: https://github.com/ston-fi/funcbox/tree/v0.0.8
[0.0.7]: https://github.com/ston-fi/funcbox/tree/v0.0.7
[0.0.6]: https://github.com/ston-fi/funcbox/tree/v0.0.6
[0.0.5]: https://github.com/ston-fi/funcbox/tree/v0.0.5
[0.0.4]: https://github.com/ston-fi/funcbox/tree/v0.0.4
[0.0.3]: https://github.com/ston-fi/funcbox/tree/v0.0.3
[0.0.2]: https://github.com/ston-fi/funcbox/tree/v0.0.2
[0.0.1]: https://github.com/ston-fi/funcbox/tree/v0.0.1