# codeless data mining
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
 <img src="21.png" alt="data" width="100"/> 
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
 <img src="22.png" alt="data" width="500"/> 
</p>