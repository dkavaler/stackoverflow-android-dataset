This repository contains data for the paper: Amount, Quality, and Latency of Answers on Stack Overflow to Questions About Recent APIs

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

# apk_list.csv

Contains a list of all unique APKs used in analysis.