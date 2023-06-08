# Call for papers website
Important dates of selected conferences in computer architecture & system fields.

## Instructions
To make changes, update the [config.toml](./config.toml) file and commit it.

Example CFP block:
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

Note:
1. The `enable` field values are as follows: 0 to hide this conference, 1 to show it, and 2 to highlight it.
2. From `open` to the `notidue`, you can fill in the date. The date format that includes timezone information is YYYY-MM-DD HH:mm:ss +/-HH:mm, with two digits for each time field. Note that the time zone behind should be the time difference from GMT time, and there must be two digits before and after the colon.
3. The `open` and `close` fields can only write dates without times.
4. You can write specific date and time for `absddl`. If you don't need to submit an abstract, you can also write "N/A".
