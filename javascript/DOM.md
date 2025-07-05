
document object model 
its an object that represents the page we see in the browser and porvides with an API to interact with it

the web browser contructs the dom when you load the page in a web browser

javascript can access the dom to dynamically change the content structure and style of the web page

---
# Element selectors

methods used to target and manipulate html elements
they allow you to selcet one or more elements from html dom

## Document.getElementbyId()
it gets the element or shows null
 
##  getElementsbyclassname()
returns an html collections
similar to an array but has less functions

![[Pasted image 20250524151243.png]]
to change something we use an index

or an enhanched for loops like
![[Pasted image 20250524151327.png]]

html collections dont have a for each function
to use it we typecast it
![[Pasted image 20250524151558.png]]

## get element by tag name

![[Pasted image 20250524151832.png]]
h4 elements and li(list) elements are seleceted
and the changed using for loop method

or we can use for each method  by type casting it like this
![[Pasted image 20250524152008.png]]

## query selector
it will show the **first** matching elemeent or null if it dosent find any matches
![[Pasted image 20250524152126.png]]


## query slector all 

results [[nodelist]] unlike html elements that are live
nodelists have a for each method no need to type cast it
they dont change
![[Pasted image 20250524152415.png]]


---
# DOM navigation

the unoredered lists

![[Pasted image 20250524153229.png]]

## firstElementChild
selects the first born childern of a group 
![[Pasted image 20250524152907.png]]
useing querry selectore all to select all the unordered lists
then using the for each method to access the first child and then change its background color 

## last element child
same stuff but of last element

## next element sibling
access the next element ie sibling of the element you slected
and if you select something then it would result in null
![[Pasted image 20250524153352.png]]

if you select an un ordered list then it would select the next **unordered list**

## previous element sibling

same stuff but for previous element 

## parent element

which ever element you select then the parent element of that element would be selected
![[Pasted image 20250524153645.png]]
the parent of fruits(unordered list) will be selected

## children

i would select all the children of the selected element 
i would selecte as an html element so you would need to typecast it as an array
![[Pasted image 20250524153835.png]]

You can also use indexes to select an element
![[Pasted image 20250524154015.png]]

---

