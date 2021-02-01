# UTF8MB4 Helper

Helper module to prevent PDOExceptions, if your database isn't able to save
utf-8 4-byte characters, but users try to insert emojis, Asian symbols or
mathematical symbols.

If that happens, you get errors like:

```
SQLSTATE[22007]: Invalid datetime format: 1366 Incorrect string value: '\xF0\x9F\x98\x80' for column...
```

The module can get uninstalled again, as soon as your database got updated to
support these 4-byte characters.

Until then you have the option to either prevent form submission with
problematic characters, or (silently) replace them on submission.

## Installation

- Install this module using the official [Backdrop CMS instructions](https://backdropcms.org/guide/modules)
- Go to admin/config/content/utf8mb4_helper and set your preferences

## Issues

Bugs and Feature requests should be reported in the [Issue Queue](https://github.com/backdrop-contrib/uft8mb4/issues)

## Current Maintainers

- [Indigoxela](https://github.com/indigoxela)

Created for Backdrop CMS by Indigoxela

## License

This project is GPL v2 software. See the LICENSE.txt file in this directory for complete text.
