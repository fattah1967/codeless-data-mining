# Knime-codeless-Al-quran-Test
## Overview
****The project is a text mining project which uses Ayah Al-Qur'an Surah Al-Fatihah for text mining by taking the text that each translator translates to find the similarity. By using the process of text mining, in text mining we used the knime program in text mining which was the first project. which the benefits of this project It is able to do a search engine that will be able to search the meaning and find the meaning of other translators as well.****
## Method
**first step Import Excel file into knime using node Excel reader.**
<p float="left">
 <img src="1.png" alt="data" width="100"/> 
</p>

## Tranform Data
<p float="left">
 <img src="2.png" alt="data" width="500"/> 
</p>

1. Using Node Column Filter.
<p float="left">
 <img src="3.png" alt="data" width="100"/> 
</p>

* to remove a column that is not removed.
<p float="left">
 <img src="4.png" alt="data" width="500"/> 
</p>

2. Using node Transpose.
<p float="left">
 <img src="6.png" alt="data" width="100"/> 
</p>

**Before**
<p float="left">
 <img src="9.png" alt="data" width="500"/> 
</p>

**After**
<p float="left">
 <img src="5.png" alt="data" width="500"/> 
</p>

3. Using node Column Combiner.
<p float="left">
 <img src="8.png" alt="data" width="100"/> 
</p>

* Combine 7 columns into one column. and one new column will be added.
<p float="left">
 <img src="9.png" alt="data" width="500"/> 
</p>

**Result**
<p float="left">
 <img src="10.png" alt="data" width="500"/> 
</p>

4. Using node Colum Filter.
<p float="left">
 <img src="11.png" alt="data" width="100"/> 
</p>

* Remove all 6 columns and leave 1. Included columns.
<p float="left">
 <img src="12.png" alt="data" width="500"/> 
</p>

**Result**
<p float="left">
 <img src="13.png" alt="data" width="500"/> 
</p>

5. Using node Column Appender + Node  Table Creator.
<p float="left">
 <img src="14.png" alt="data" width="100"/> 
</p>

* These 2 will add a new ID.
<p float="left">
 <img src="15.png" alt="data" width="100"/> 
</p>

6. Using node String Manipulation.
<p float="left">
 <img src="16.png" alt="data" width="100"/> 
</p>

* Delete the dash or this – dash because it is not necessary.

**Before**
<p float="left">
 <img src="17.png" alt="data" width="300"/> 
</p>

**After**
<p float="left">
 <img src="18.png" alt="data" width="300"/> 
</p>

## Text Proccessing
<p float="left">
 <img src="19.png" alt="data" width="500"/> 
</p>

1. Using node String to document .
<p float="left">
 <img src="20.png" alt="data" width="100"/> 
</p>

* to change string to document 
<p float="left">
 <img src="21.png" alt="data" width="70"/> 
</p>

2. Using node Column Filter .
<p float="left">
 <img src="3.png" alt="data" width="100"/> 
</p>

* to remove unuse column 
<p float="left">
 <img src="22.png" alt="data" width="500"/> 
</p>

**Result**
<p float="left">
 <img src="23.png" alt="data" width="300"/> 
</p>

3. Using node Punctuation Erasure.
<p float="left">
 <img src="24.png" alt="data" width="100"/> 
</p>

* to remove punctuation (? , . () , : ; "") 
 
 **Before**
 <p float="left">
 <img src="25.png" alt="data" width="700"/> 
</p>

**After**
<p float="left">
 <img src="26.png" alt="data" width="500"/> 
</p>

4. Using node Case Converter.
<p float="left">
 <img src="27.png" alt="data" width="100"/> 
</p>

* to change all character to be lowercase letter

5. Using node Stop Word Filter.
<p float="left">
 <img src="28.png" alt="data" width="100"/> 
</p>

* to remove stop word.

6. Using node POS Tagger, node Stanford.
<p float="left">
 <img src="29.png" alt="data" width="150"/> 
</p>

* to separate word Part of speech(nouns ,verbs , adverb etc.)

7. Using node Standford Lammatizer.
<p float="left">
 <img src="30.png" alt="data" width="100"/> 
</p>

* to make the verb to be base form

8. Using node Bag of Word Creator .
<p float="left">
 <img src="31.png" alt="data" width="100"/> 
</p>

* to create bag of word

## Model
1. Using Node TF Node IDF.
*  Model Use TF and IDE to find word frequencies.
2. Using Node Math Formula.
*  To TF and IDF are multiplied gether for more accurate results.
<p float="left">
 <img src="32.png" alt="data" width="300"/> 
</p>

**Result**
<p float="left">
 <img src="33.png" alt="data" width="500"/> 
</p>

3. Using Node Document Vector.
<p float="left">
 <img src="34.png" alt="data" width="100"/> 
</p>

* 
**Result**
<p float="left">
 <img src="35.png" alt="data" width="700"/> 
</p>

## Similarity View(TF-IDF)
<p float="left">
 <img src="36.png" alt="data" width="700"/> 
</p>

1. Add Column And Sort Column By ID
<p float="left">
 <img src="37.png" alt="data" width="200"/> 
</p>

2. Similarity View
<p float="left">
 <img src="38.png" alt="data" width="500"/> 
</p>

* Determines the translator to compare the similarity use Column ID.
