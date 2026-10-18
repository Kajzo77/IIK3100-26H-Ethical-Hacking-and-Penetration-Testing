# Home Task 1: 
### Earth book / RSA

Somebody left an XLSX file on NTNU domain, can you figure out the file author’s name?

Flag format:FLAG{Author First Name Only}

### Writeup
1. Open the search engine duckduckgo and use the dork:\
   site:ntnu.no filetype:xlsx
   
2. The dork includes:\
   site:ntnu.no - restricts the results to ntnu domain.\
   filetype:xlsx - limits the results to xlsx files.
   
3. The search engine duckduckgo returns multiple links to xlsx files within ntnu.no domain.
 
4. Use the challenge title as a hint: \
   Earth Book - the file title in english
   
5. Find a link that has the word "jordbok" in its url. "Jordbok" is the norwegian word for "Earth Book".

6. Copy the link of the chosen file.
   
7. Use the webtool ExifTool and insert the file link to extract metadata.\
   https://exiftools.com/

8. The metadata will include the name of the author, which is Ivar Ståle Ertesvåg. Use his first name to construct the flag.

The file link:\
https://ivarse.folk.ntnu.no/avskr/jordbok1626_kyrkjegods.xlsx

The flag:\
FLAG{Ivar}
