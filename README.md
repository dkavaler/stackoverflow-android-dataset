This repository contains data for the paper: Amount, Quality, and Latency of Answers on Stack Overflow to Questions About Recent APIs

# play_crawler.zip

Contains source code and a compiled jar file to crawl the Google Play store for free applications.

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

# android_api_change_dates.csv

List of each Android API level studied, and their release date.

# android_api_changes_wdate.csv

List of all API changes for each API level, with the given change type (when compared to the prior API level).
APIs can be added (1), removed (2), or changed (3).

| Column | Description |
| ------ | ----------- |
| level | API level of the given API's change |
| date | Date of the given API's change |
| fully_qualified_classname | Fully qualified classname for the API |
| change_type | 1, 2, or 3, corresponding to added, removed, or changed |

# api_callcounts.gz

Contains a csv file (api_callcounts.csv); list of function invocation counts for each APK, for each Android API.

| Column | Description |
| ------ | ----------- |
| apk | Name of APK |
| api | API the count is for |
| callcount | Number of calls to the given API in the given APK |


# links_all.RData

An R data.table containing each linked Stack Overflow post id, along with the linked API, the way it was linked (e.g. through a code link), and
the API level of the linked class, based on the post's creation date.
