### Useful-tipsORcode

#### **Linux**

*Remove line with a pattern in it*

```sh
sed -n '/__/!p' CGI-1.counts >> CGI-1.countsM
```
Print every line from a file (here: CGI-1.counts) except lines with pattern "**__**" in them.  A way to get rid of a line with a specififc pattern.

Especially the htseq-count files have some lines at the end of the file with "**__**" at the end and they need to be removed before downstream analysis. The ouput file has to be seperate name then the input file hence the **M** in output file name. The **M** can be removed before use if desired.
