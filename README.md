# Address extraction

## Solution
 This repo aims to extract address elements from raw text 
 
 For example
 ![image](https://user-images.githubusercontent.com/65607884/152207068-ec0c2444-57ae-413b-95c7-3cc1c8dc7aa9.png)
 
 1. Clean text and extract some information first including Zip Code, House number, Moo and list_other (which includes subdistrict, district, province and other info but not yet extracted)
 2. Search each element and compare with Thai governace subdistrict-level local name data.
 3. Correct misspelled tokens using Levenshtein distance. So, there would be no concern about an incorrect text.
    
    Source : https://en.wikipedia.org/wiki/Levenshtein_distance#:~:text=Informally%2C%20the%20Levenshtein%20distance%20between,considered%20this%20distance%20in%201965.
    
 **P.S.** : This repo just only display about the application of autocorrection. So, there would be a problem if you have the big size of subdistrict-level data due to a big O.
