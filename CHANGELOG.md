### 0.9.1
- Updated `scut-font-face` so users can enter there own `$formats` list, if they don't want to include all font-file-formats.

### 0.9.0
- Documented `scut-reset` so that others might understand.
- Added `$no-margin` variable to list mixins, with the default value `true`.
- Made `scut-font-face`'s argument `$weight` optional.
- Removed inner element from `scut-ratio-box`, as the user can add it herself if she wants it (and she may not want it).
- Exposed the `$scut-rem-base` default value to users.

### 0.8.0
- Fixed a bug preventing the results of `scut-em` and `scut-rem` from being used in calculations.
- Added `scut-truncate`.
- Deleted "tests" in repository. Devs should use Codepen. It's easy.
- Updated `scut-reset`. Some substance-changes and specific resets are now excludable.

### 0.7.1 and 0.7.2
- Bug fixes.

### 0.7.0
- Updated `scut-list-unstyled` for less aggressive resetting; modified related utilities to fit.
- Updated `scut-fill` for two different filling approaches: all coordinates = 0 or width/height = 100%.
- Updated `scut-em` to accept lists of pixel-values and exposed the `$scut-em-base` default value to users.
- Added `scut-rem` and `scut-rem-fallback`.
- Added `scut-list-custom`.
- Added `scut-center-trasform` and `scut-vcenter-tt`.

### 0.6.0
- Added RubyGem config so Scut can be used as a standard Compass extension.
- Modified `scut-margin` and `scut-padding`.
- Added `scut-center-block`.
- Changed `scut-hide-text` to `scut-image-replace` and added `scut-hide-visually`.
- Moved `scut-triangle` and `scut-circle` to General category; removed `scut-foursquare`; and removed Shapes category.
- Replaced block comments with in-line comments.

### 0.5.0
- Added `scut-border`.

### 0.4.1
- Fixed bug with `scut-foursquare`: it requires `box-sizing: border-box`.

### 0.4.0
- Started changelog!