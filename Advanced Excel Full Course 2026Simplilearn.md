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



####  (eg sheet2)

-->there might some condition where you compare with two col and compare there are not complete it may have some part of the it's compare thing so we want those will be true 
-> so for that we will use VLOOKUP again but put while card thing with that compare cell data --> "*" --> "this means if there anythings when you comparing with first cell and other cell or anything extra rather than the actual cell please try to consider it
eg ; =VLOOKUP("*"&A1&"*", B:C, 2, FALSE)

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

## 1. How to Freeze Rows in excel
* (like you want to freeze header to you will refrense the data after scroll down)

* also if i want to freeze a column data, when scrolling left to right

* so for that you have to select a cell where above of that row and just left col will freeze for that you have to go -> <view> menu -> there is option (freeze panes);; so there is option we can freeze row only , column only or both


## 2. we have a col where amount of money are there we want convert those into **Amount in words**

* there is not any pre-define fn ;; but we can build such fn using excel bba and VBA

so you can create a micro using developer option but developer option is not readly availble in microsoft excel;; to activate developer option go to -> <home> -> <option> menu at the last -> go to <custemize Ribbon> -> at the second drop-down menu you will see ; by default will not be checked ;; please click and make it checked 


* now go to <developer option> -> go to <visual basic> -> go to <insert> to insert new micro -> <module> now new micro window is availble for you , now paste you can which you catched for number to word convert by VBA

## 3. let you want to create one single cell for all the employees in you country ;; like there first name, last name and including there gmail id

* so you can do it by **combine operation in excel**
`=first_name_cell_pos &(emphsent sign) last_name_cell_position : email_cell_pos`
* also want to give some spaces
`=first_name_cell_pos &" "&(emphsent sign) last_name_cell_position &" "& email_cell_pos`

## how to merge cells in excell
* let we have sales data of john in january month
* now we have sales data  same for john for three months 

* now you want to merge these three months and write it down quater1
* basically remove those three month header (or merge them) and put -> only Quarter 1

`<home> -> go to aligment group and  select <merge and center>`

* there is diff merge option first we used which was merge and center 

* now if you have multiple row with diff cells and and each row has Review for each month and you want each row will merge and don't want to go each row on by one just select all and select option **merge across**

## 3. (how to use date-time fn)

* you can easly get today data using <today> fn press enter

* but there is some problem with these kind of approch , is when ever you open this sheet again the day has been changed to that day date;; so that date always vary 

* so that should not vary ;; there is another shortcut way to use date-time fn ;; a key ward short to add todays date -> `ctrl+ ;` ;; and this will not be chaged 

* there might also you want to add time to spread sheet;; `ctrl+ shift + ;` so then you will have time

* and these date and time will resame constant

## 4. (date formats)
* there might not be you date in date format so converting those text -> date type you just have to go `<data> -> text to column`

* you may want to change format of date type so -> `select that col and -> right click ->  format cell option ;; also can change date format according to diff country there `

* now if your client don't want date format they want only month so at same place and choose `custom -> select only month and year`

## 5. (how to calculate **age**)

* if you have date col , so using it how to calculate age --> using Datedif fn -> `=datedif(cell_where_date_is, today_fn, if_you_want_to_cal_age_in_term_of_days->"d" or if month_then->"m" or 'y')`

1:1:0