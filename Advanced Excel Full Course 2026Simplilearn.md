https://www.youtube.com/watch?v=8Ob8Hre_SnI&t=1202s

# Day1
what is me
-> me is software product designed and developed by Microsoft for storing data in an organised way. 

-> ms is also capable to manipulate data through mathematical functions

-> ms is also usedto extract insights from data and represent the visualization using graphs and charts

1. you have first 
-> tool bar menu
-> tool bar ribbons ( eg home)
-> tool bar groups --> tool bar more options


2. we have cell and address 
3. at the bottom we have sheet tracker (you can use any number of sheet ) and sheet size


## demo inventory in excel
-> using mc to create a sheet for employees in a company 
-> want to use new column or row use --> insert option present click on right of your mouse

--> convert text column to lower case and upper case 
-> use =Lower

20:min

# Day2
## 1 if we want to add a row in the dataset : 
-> same right click and click insert
--> if you want to add multiple row just select that many row and click right + insert

--> lly you can add a col --> always remember excel sheet add a new col of it's left side (lly right click + insert)


## 2 you have any money column and you want to add it's money sign (like $, rupee etc) so this work is easy if you have only 3-4 row but if you have multiple row you can go manually and add --> so there is multiple method to do it
--> click on col number (A, B, C...) --> so entire col is selected or --> click anywhere in that col and ctrl+ space 

--> lly if you want to select a row 1. directly click on it's row number (1, 2...)
or shift+ space

--> now if want to select all the cells which have data -> first select the cell  then ctrl+ space + lower_arrow_key --> it will select all the cells which have data

--> lly for row --> ctrl + shift + right_arrow

--> now come to our question adding money symbol first select that col then go--> Power Pivot -> general --> currency -> choose your currency


## 3 now comparing two diff columns or multiple columns is important jobs when you working as data analytics
-> now we have two col -> col1 and col2 and i want to compare both of them

-> first way (simple) --> use build-in conditional formatting which comes excel by default -> only have to do that select all the data --> navigate to home -> go to styles -> conditional formatting -> Highlight cell Rule -> duplicate values --> after that you will get box where you have to choose what you want to see duplicate cells in both col or unique ;;or also can find unique value which is only present in col1 not in col 2

-> second way --> =(select_your_first_col_cell)=(select_your_sec_col_cell_) -> if they match then give true else false

(learn to use 'If' operator)
-->if you want to add some other features like also want to check wether these col value data exist or not then compare --> =IF(A2=B2, "Found", "Not found")

--> Third way to compare (using lookup fn) -> used simple vloopup fn to compare both of the cell
`=VLOOKUP(one_col_value_want_to_compare, range_of_col_where_you_want_to_compare (then press F4 for log them),1 (bz you want data from col 1 , 0 (bz you want exact match so )
--> here if the element get in col1 then it will be printed in result but else it will give error (also we can handle this error add IFERROR simply write not found)
eg ; =VLOOKUP("*"&A1&"*", B:C, 2, FALSE)


####  (eg sheet2)

-->there might some condition where you compare with two col and compare there are not complete it may have some part of the it's compare thing so we want those will be true 
-> so for that we will use VLOOKUP again but put while card thing with that compare cell data --> "*" --> "this means if there anythings when you comparing with first cell and other cell or anything extra rather than the actual cell please try to consider it


#### eg(sheet3)

# 2 How to convert Rows to Columns in execl
--> first way select all the cells copy it first (ctrl+ c) --> you will see a paste option at the top left most side -> navigate to paste special --> you will see transpose option

# 3 second way --> go to the function bar --> write -> TRANSPOSE(SELECT_THE_ARRAY) ;; transpose it basically an array fn in execel


# eg (sheet4)

## if you want to hide some cols
--> go to  -> data option -> click on group option now you can hide this col using that minising option

--> also you can ungroup them --> for that you have to select those col or row and go same 'data' -> ungroup



# eg (sheet5)

## I have some sample data on my spreadsheet and does have some blank rows now , how i elemenate these blank rows
1. manually go and delete them
2. go to the find_and_select_options -> go_to_special -> now select the blank option (after that all the blank row will be selected) -> now hold ctrl+ (-key) --> you will be having the option of deleting the cells (select the entire row) so we have selected rows with blank data --> now the you will see the cells will be shifted

3. what , what if we have some data in the row and other cells of that row are blank, so in such scenario how do we eliminate data
--> so for that we have a simple logic for it , all we have to do is add another col which count the number of cells(have data) in a row
--> for that we use ''''COUNTA''' --> AFTER THAT select all using -> (ctrl+ a) --> then go '''filter''' option and now all the header have filter option you can now filter in the basis of it's value

--> so if you want to delete row which have that count value are zero direct select those by filter and delete( select all ctrl+ a and delete (ctrl+ (-key))



### 40:00 min


