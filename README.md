# TSM-Localization

This repository contains all the localization files for the TradeSkillMaster World of Warcraft addon.

## Contributing

**NOTE:** By submitting a contributation and/or participating in any discussion within this repository, you acknowledge that you've read and agree to the [Contributor Agreement](CONTRIBUTOR_AGREEMENT.md).

### Submitting Changes

To contribute an update to the localized strings, follow these steps:
1. Download the `.txt` file for the locale you want to change from this repository.
2. Find the line within the file for the string you want to change. For example:

    ```L["Scanning (%d Items)"] = "Scanning (%d Items)"```
3. Update the part after the `=` to match what the string should say in the language you are updating. For example:

    ```L["Scanning (%d Items)"] = "Analyse (%d objets)"```

4. You can test your changes in the addon by open the appropriate file for the locale you want to change within your local copy of the addon. For example, `TradeSkillMaster/Locale/frFR.lua` for French and replacing all lines between the `-- LOCALE STRINGS START HERE` and `-- LOCALE STRINGS END HERE` lines in the file with the contents of your updated .txt file.
5. To submit your changes to the project, open either an issue or a pull request with the contents of the new .txt file.

### Tips

* Make sure not to include any extra whitespace at the beginning or ending of the translated string.
* `%d` or `%s` are format specifiers which will dynamically be replaced by a value. For example, in the string `"Scanning (%d Items)"`, the `%d` will be replaced by a numeric value before getting displayed. If there are multiple format specifiers in a string, the order must be maintained.
* A `%s` format specifier may also be used to change the color of a portion of a string, with the portion either ending in another `%s` or in a `|r`. The position of these should also be maintained as appropriate.
* Try and keep the length of the text the same size as or smaller than the original English phrase to ensure it'll fit nicely in the allotted space in the UI.

## License

Copyright (C) 2025 TradeSkillMaster LLC

All Rights Reserved
