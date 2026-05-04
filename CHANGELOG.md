# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.2] - 2026-05-04

### Added

- `wpcs_input_nvs` for input not validated nor sanitized (`WordPress.Security.ValidatedSanitizedInput.InputNotValidatedNotSanitized`)

## [1.2.1] - 2026-05-04

### Added

- `wpcs_unused_param` for unused function parameters (`Generic.CodeAnalysis.UnusedFunctionParameter.Found`)

## [1.2.0] - 2026-05-04

### Added

- `wpcs_var_snake` for non-snake_case variable names
- `wpcs_prop_snake` for non-snake_case property names
- `wpcs_hook_underscore` for hooks without underscores
- `wpcs_non_yoda` for non-Yoda conditions
- `wpcs_loose_equal` for loose equality comparisons
- `wpcs_safe_redirect` for wp_redirect() usage
- `wpcs_dev_functions` for debugging functions
- `wpcs_method_name` for invalid class method names
- `wpcs_commented_code` for commented out code blocks
- `wpcs_textdomain` for missing translation text domains (renamed from `wpcs_i18n_textdomain`)
- `wpcs_file_name` for non-standard file names
- `wpcs_escape` as alternative to `wpcs_xss`

### Fixed

- Update `wpcs_loose_comparison` to use `Universal.Operators.StrictComparisons.LooseComparison` (WordPressCS 3.0.0)
- Update `wpcs_precision_alignment` to use `Universal.WhiteSpace.PrecisionAlignment.Found` (WordPressCS 3.0.0)
- Update `wpcs_spelling` to use `WordPress.WP.CapitalPDangit.MisspelledInText` (WordPressCS 3.0.0)

## [1.1.0] - 2022-09-10

### Added

- `wpcs_csrf_recommended` snippet for skipping recommended nonce verification

### Changed

- Update precision alignment rule to `WordPress.WhiteSpace.PrecisionAlignment.Found`
- Update capital P dangit rule to `WordPress.WP.CapitalPDangit.Misspelled`
- Update global variables override rule to `WordPress.WP.GlobalVariablesOverride.Prohibited`
- Rename `wpcs_cache` to `wpcs_db_cache`
- Rename `wpcs_csrf` to `wpcs_csrf_missing`
- Rename `wpcs_function_name` to `wpcs_fn_name`
- Rename `wpcs_preparedsqlplaceholders` to `wpcs_db_preparedsqlplaceholders`
- Rename `wpcs_slow_query` to `wpcs_db_slow_query`
- Rename `wpcs_unprepared_sql` to `wpcs_db_unprepared_sql`

## [1.0.3] - 2022-01-15

### Fixed

- Correct various snippet definitions

### Changed

- Reorder snippets alphabetically

### Added

- `wpcs_function_name` snippet for invalid function names

## [1.0.2] - 2021-10-10

### Fixed

- Fix "input var ok" snippet (`wpcs_input_var`)

## [1.0.0] - 2021-10-06

### Added

- Initial release
