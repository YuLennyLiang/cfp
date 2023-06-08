# Call for papers website
Important dates of selected conferences in computer architecture & system fields.

## Instructions
To make changes, update the [config.toml](./config.toml) file and commit it.

Each conference CFP has the following fields:

- The `enable` field has three values: 0 means that the conference will not be displayed on the website, 1 means it will be displayed normally, and 2 means it will be highlighted in the "Featured CFPs" section at the top of the website. Note that only one conference can have this field set to 2; otherwise, there may be problems with countdown timers (the countdown for other conferences on the website is shown in days, while Feature CFP shows hours, minutes and seconds).
- The `name` field is for the name of the conference.
- The `rank` field is for categorizing international academic conferences recommended by CCF.
- The `site` field is for providing a link to the conference's official website.
- The `open` field indicates when the conference begins.
- The `close` field indicates when it ends.
- The `absddl` field indicates when abstract submissions are due. If there isn't one, you can write N/A. Do not write anything else or an error may occur (because special processing is required for timelines at top of webpage).
- The `submddl` field indicates when formal papers are due.
- Finally, the `notidue` field refers to date of acceptance notification.

For all fields related to dates and times mentioned above, the specific format should follow this pattern: 2006-01-02 15:04:05 -07:00. That is year-month-day hour-minute-second followed by time difference relative to UTC timezone (-12~+14). Please convert according to instructions provided by each individual conference website. It should also be noted that every item in date-time format must consist of two digits. Below are some examples showing how different formats can be used; you can choose whether or not to include both date and time information depending on your needs.

```
[[params.cfp.list]]
enable = 1
name = "FAST"
rank = "A"
site = "https://www.usenix.org/conference/fast22/call-for-papers"
open = "2022-02-21"
close = "2022-02-24 23:59:59"
absddl = "N/A"
submddl = "2021-09-23 23:59:59 -07:00"
notidue = "2021-12-10"
```
