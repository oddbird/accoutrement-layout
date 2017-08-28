Changelog
=========

3.0.0 – UNRELEASED
------------------

- BREAKING: Remove `$inherit` option from `box-sizing`
  (because it's a bad idea to inherit box properties).
  You can still replicate the behavior by setting box-sizing on the root,
  and passing `inherit` as an argument to the mixin.
- BREAKING: Remove `micro-clearfix` in favor of `clearfix` alias.
  The only other reliable clearfix is `overflow: hidden` -
  and we don't need a mixin for that.
- BREAKING: Rename `$_accoutrement-query-context` and make it private.
- BREAKING: Rename `$_ACCOUTREMENT-ASPECT-RATIOS`
  to make it private, and signify that it remains constant.
- BREAKING: Remove automatic `browser-ems` conversion,
  in favor of explicit breakpoint values/units.
  For unit-conversion and more helpful size-utilities,
  see [Accoutrement-Scale](http://oddbird.net/accoutrement-scale/).
- BREAKING: Remove `stretch` mixins, as an over-specific use-case.
- NEW: Add a single `position` mixin using the common TRBL syntax
  to provide a shortcut for positioning properties
  (`top`, `right`, `bottom`, `left`, and `position`).
