###Useful-tipsORcode

**Linux**

Print every line from a file (here: CGI-1.counts) except lines with pattern "**__**" in them.  A way to get rid of a line with a specififc pattern.
Especially the htseq-count files have some lines at the end of the file with "**__**" at the end and they need to be removed before downstream analysis.

```sh
sed -n '/__/!p' CGI-1.counts >> CGI-1.countsM
```
