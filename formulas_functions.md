<COUNTIF: A function that returns the number of cells that match a specified value.>

- =COUNTIF(range,"value")
  > Ej. =COUNTIF(I2:I72, "<100>")

---

<LEN: A function that tells you the length of a text string by counting the number of characters it contains.>

- =LEN(range)
  > Ej. =LEN(I2)

---

<LEFT: A function that gives you a set number of characters from the left side of a text string.>

- =LEFT(range,numbers of characters)
  > Ej. =LEFT(B2,4)

---

<RIGHT: A function that gives you a set number of characters from the right side of a text string.>

- =RIGHT(range,numbers of characters)
  > Ej. =RIGHT(T4,6)

---

<MID: A function that gives you a segment from the middle of a text string.>

- =MID(range,reference starting point, number of middle characters)
  > Ej. =MID(T4,3,2)

---

<CONCATENATE: A function that joins together two or more text string.>

- =CONCATENATE(item 1, item 2)
  > Ej. =CONCATENATE(T4,A3)

---

<TRIM: A function that removes leading, trailing, and repeated spaces in data.>

- =TRIM(range)
  > Ej. =TRIM(T4,A3)

---

<VLOOKUP: Vertical Lookup, A function that searches for a certain value in a column to return a corresponding piece of information.: A function that removes leading, trailing, and repeated spaces in data.>

- =VLOOKUP(data to look up,'where to look' !Range, column, false)
  > Ej. =VLOOKUP(A2,'Sheet 2'!$A$2:$B$31,2,FALSE)

---

<SPLIT: Split the text by a delimiter character.>

- =SPLIT(text,delimiter,[split celd], [delete spaces])
  > Ej. =SPLIT(A)

---


<COUNTA: Counts the total numbers of values within a specified range.>

---

<CASE-Statement: The CASE statement goes through one or more conditions and returns a value as soon as a condition is met.>

---
<IMPORTRANGE: Import and page data from one sheet to another and updates de data automatically.>

- =IMPORTRANGE(spreadsheet_url, range_string)
  > Ej. 
    =IMPORTRANGE("https://docs.google.com/spreadsheets/d/1TmSoTCeMdY5RT7IsA9MUflg-QiOyXK4_zyCUZgkPZMY/edit?gid=0#gid=0","Sheet1!A2:C25")

---
<QUERY: Allows to make SQL querys on a sheet.>

- =QUERY(Sheet and Range, "Select *")
  > Ej. 
    =QUERY('Association ABC memberships'!$A$1:$I$50,"select A,C  ")

---
<FILTER: Filter the data where a condition is met.>

- =FILTER(range, condition1, [condition2, ...])
  > Ej. 
    =filter(A2:C20,B2:B20 <1000)

---