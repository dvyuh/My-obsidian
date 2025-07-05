![[Pasted image 20250519134303.png]]

![[Pasted image 20250519134317.png]]

you can also add a function in an object
![[Pasted image 20250519134902.png]]

---
## This function
![[Pasted image 20250519135239.png]]

**this function does not works with [[Function Expression#Arrow Function|Arrow function]]  

you have to use normal function 
![[Pasted image 20250519140454.png]]

---


## Constructor
a special method for defining the properties and method of objects
![[Pasted image 20250519141704.png]]
this is a constructor 

this constructor is used to model other objects like this
![[Pasted image 20250519141736.png]]

---

## Class 
class provide a more structured way to work with objects compared to traditional constructor function 
![[Pasted image 20250519142832.png]]

![[Pasted image 20250519143201.png]]

---
##  Static

![[Pasted image 20250519143349.png]]

anyhting that is stactic belongs to the class not the object in the class

Example1
![[Pasted image 20250519144130.png]]

Example2
![[Pasted image 20250519144431.png]]
in this example there is both static and constructor in a class

when u use user1.count it wont work as static is inside a class(it belongs to a class)
hence we use user.usercount 

---
## Inheritence
allows a new class to inherit properties and method from existing class (parent=>child) helps in code reuseability

this is the parent class
![[Pasted image 20250520111325.png]]
these are the classes that use the parent classes
![[Pasted image 20250520111354.png]]
we can also specify  new methods to specific classes like in rabbit run method
this wont affect the fish class

i wont need to specify the properties again and again

---

## Super keyword

![[Pasted image 20250520112808.png]]
the super keyword is used to get name and age of different class

---

## Getter and setter
getter is a special method that makes a property readable
setter is  a special method that makes  a property writable

![[Pasted image 20250520115829.png]]
using set  to validate the input ie the value passed in is a number
get will also be used along side set.

as the properties is set we will use get to get the set properties


---

## Destructuring 

extracting values from objects and arrays and objects, then assign them to variables in a conveient ways
{} object destructuring
[[Arrays]] destructuring

### swaping values of 2 variables
![[Pasted image 20250520130334.png]]

### swap two elements in an array

![[Pasted image 20250520130641.png]]

### assign array elements to variables
![[Pasted image 20250520130952.png]]

the colors in first is the first colors 
then using ... too make a new array


### Extract values from objects
![[Pasted image 20250520131408.png]]


### destructure in function parameters
![[Pasted image 20250520131553.png]]


---


## Nested objects

used to create complex data structures 

to see a property in a nested object person-> address use . to see it
![[Pasted image 20250520132131.png]]


Example 2
![[Pasted image 20250520132801.png]]

Address object is a nested object in person object

---

## Array of objects

previously we made an array of strings or numbers now with objects

then use a for each function to display every fruit name 
![[Pasted image 20250520134459.png]]

**using a reduce function**

![[Pasted image 20250520134750.png]]

---
## sorting method in aaray of objects

used to sort elements of an array ini place 
![[Pasted image 20250520135524.png]]

for sorting numbers
![[Pasted image 20250520135538.png]]

for sorting strings alphabetically
![[Pasted image 20250520135633.png]]

---
## Shuffleing method in elements of an array

![[Pasted image 20250520140149.png]]

---

## Date object
objects that contain the values that represent dates and time theese date objects can be changed and formatted]

![[Pasted image 20250520144258.png]]

