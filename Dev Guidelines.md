# foxPEP - Development Guidelines
1. Unless disabling outright / reconfiguring to none (0) or setting to unlimited (-1), most integer preferences should be modified based upon multiples of the original value (Ex. if 8, then 16, 24, 32, etc.).

2. "Larger amounts are better" / "shorter delays are desired" is not a one-size-fits-all model.

3. Generally, the fewer preference alterations there are, the more efficiently the browser will respond.

4. Final releases must be packaged from a Linux or BSD environment, as Windows and macOS will autonomously place index files in the release folder. Xarchiver is the recommended packaging tool.
