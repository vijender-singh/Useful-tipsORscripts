# Useful-tipsORcode

**Linux**
Print every line except line with pattern "**__**" from a file.  A way to get rid of a line with a specififc pattern.
Especially the htseq-count files have some lines with "**__**" at the end and they need to be removed before downstream analysis.

```sh
sed -n '/__/!p' CGI-1.counts >> CGI-1.countsM
```
