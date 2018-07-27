# CACParser
awk script for generating csv file from dwzrv show results.


requirements:
poppler-utils ( apt-get install poppler-utils )  
or
xpdf tools from https://www.xpdfreader.com/download.html
gawk

usage:
1. download Show result from dwzrv
2. convert pdf with: pdftotext -raw -enc UFT-8 filename.pdf
3. gawk  -f CACParser.awk -v title="Tournament Name" filename.txt>out_filename.csv

TODO:
result (e.g. v1 CAC BR BIS Landssieger) is currently just a string. could be separated in Note|Place|entitelments|titels|show-result


