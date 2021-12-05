# linux-hwmon-applesmc
[PATCH] hwmon: (applesmc) Add DMI product matches for Intel-based Xserves (non-RackMac*,*)

This is a patch submission for [torvalds/linux](https://github.com/torvalds/linux).  For small projects not requiring a pull request, or where maintainers prefer e-mail patch submissions, I keep copies here for reference/download.

- File: ./drivers/hwmon/applemon.c
- Submission Date: 2020-11-28
- Commit Date: 2020-12-02 (Linux 5.11)

Summary: applesmc did not previously check for XServe hardware in the 'Product Name' field in the DMI table, resulting in broken hardware management functionality (i.e. [linux-on-mac/mbpfan](https://github.com/linux-on-mac/mbpfan)).
