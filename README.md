This repository contains data for the paper: When Stack Overflow Slows Down: Latency of Answers to Questions About New Android APIs.

# post_data.gz (post_data.csv)

Columns correspond to Table 1 in the paper.

# api_data.gz (api_data.csv)

Columns: apk, gatherdate, api, callcount
Note: Some APIs will not correspond exactly to actual Android APIs, as some APKs are obfuscated and partially match a real Android API name. These can be filtered out by cross-referencing with a real list of Android APIs, which was done in our work.
| Column | Description |
| ------ | ----------- |
| apk | Name of the APK gathered from the Google Play store |
| gatherdate | Date that the APK was gathered by our crawler |
| api | Fully qualified class name for an API call. |
| callcount | Number of calls within the specified APK to the given API |