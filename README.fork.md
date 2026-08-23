# Tategumi fork note

This fork follows [m-tky/crengine](https://github.com/m-tky/crengine) for the
KOReader tategumi build.

Its downstream vertical-layout change fixes Japanese punctuation disappearing
at the bottom of a column. Punctuation retained there by kinsoku may paint past
the regular content boundary by no more than one effective JFM slot. The
allowance covers closing brackets, commas, full stops, middle punctuation,
colons, semicolons, question marks, and exclamation marks. Ordinary text and
opening punctuation remain clipped.

The behavior is covered by KOReader emulator regressions for
`」、。・，．：；！？` and was verified with Source Han Serif on a PocketBook
Touch HD 3.
