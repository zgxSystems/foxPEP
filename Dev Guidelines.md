# foxPEP - Development Guidelines
1. Unless disabling outright / reconfiguring to none (0) or setting to unlimited (-1), most integer preferences should be modified based upon multiples of the original value (Ex. if 8, then 16, 24, 32, etc.).

2. Generally, the fewer preferences there are, the more efficiently the browser will respond.

3. No modifications may be implemented that outright breaks FF 38+ / 27+.

4. Final releases must be packaged from a Linux or BSD environment, as Windows and macOS will autonomously place index files in the release folder. Xarchiver is the recommended packaging tool.

5. sb.scorecardresearch.com should not be included in the blocklist, as some websites will use the presence of this connection to check for an ad blocker. If its connection is not detected, the website may choose to withhold content. To avoid this, making use of uMatrix is helpful when debugging the blocklist to confirm what calls sites make to which servers.
