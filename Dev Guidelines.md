# foxPEP - Development Guidelines
1. Unless disabling outright / reconfiguring to none (0) or setting to unlimited (-1), most integer preferences should be modified based upon multiples of the original value (Ex. if 8, then 16, 24, 32, etc.).

2. "Larger amounts are better" / "shorter delays are desired" is not a one-size-fits-all model.

3. Generally, the fewer preference alterations there are, the more efficiently the browser will respond.

4. As a rule, the browser will accept any preferences it recognizes and ignores everything it doesn't. This is why it's OK to include preferences specific to one environment in the main file, as inapplicable environments will simply discard what does not apply.

5. In accordance with the aforementioned standard, it is better to disable only (ex. app.update.enabled) rather than (ex. app.update.enabled) + (ex. app.update.auto), as the ".enabled" / ".disabled" suffixes function as master kill switches of the features in their entirety, thus effectively rendering further alteration of prefixing features redundant.

6. Final releases must be packaged from a Linux or BSD environment, as Windows and macOS will autonomously place index files in the release folder. Xarchiver is the recommended packaging tool.

7. Standard Firefox versions use the *default-release* profile folder and will ignore *default-esr*. Firefox ESR versions use the *default-esr* profile folder and will ignore *default-release*.
