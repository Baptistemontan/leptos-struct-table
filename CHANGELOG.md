# Changelog

## [0.7.1] -

### Changes

- Added generic error type to `TableDataProvider`
- Fixed sorting for tables with skipped fields

## [0.7.0] - 2024-02-08

### Features 🚀

- Virtualization — Only elements that are visible are rendered (with some extra for smooth scrolling).
  - Other display acceleration strategies like infinite scroll and pagination are implemented as well. 
- Caching — Only rows that are visible are requested from the data source and then cached.
- Error handling — If an error occurs while loading data, it is displayed in a table row instead of the failed data.
- Easy reloading — The data can be reloaded through the `ReloadController`.

### Breaking Changes 🛠️

Everything? - sorry. This release is like half a rewrite with much less macro magic.
Please check the docs and examples.

## [0.6.0] - 2023-11-02

### New Feature 🎉

- Support for generic structs

### Fix 🐛

- Fixed `#[table(skip_sort)]` on fields

## [0.5.0] - 2023-10-20

### Breaking Changes 🛠️

- Added `on_change` events to support editable data (see new editable example)

### Fixes 🐛

- Fixed selection with `key`s that are not `Copy`

### Other Changes

- Modified REST example to include sorting


## [0.4.0] - 2023-10-02

- Updated to leptos 0.5

## [0.3.0]

- Updated to leptos 0.4

## [0.2.0]

- Updated to leptos 0.3
- Deactivated `default-features` of leptos
- New class provider `BootstrapClassesPreset`
- New example `bootstrap`
- Added `thead` and `tbody` with customizable renderers
- Added `getter` and `FieldGetter<T>` with new example