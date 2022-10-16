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

* Before
<p float="left">
 <img src="9.png" alt="data" width="500"/> 
</p>

* After
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

* Result
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

* Result
<p float="left">
 <img src="13.png" alt="data" width="500"/> 
</p>
