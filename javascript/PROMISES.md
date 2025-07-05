An [[Objects]] that manages [[Asynchronous code]]  operations.

wrap a promise object around async code
"i promise to return a value"

pending -> resolved or rejected

new promise((resolve,reject) => {asynch code})

suppose there are thee functuons
![[Pasted image 20250526124822.png]]

**Now we'll use promises to make it in order to first walk then kitchen then trash**


![[Pasted image 20250526125312.png]]
resolve means if the function is done then this will occur if it does not then the reject function will occur

like this
![[Pasted image 20250526125531.png]]



**This is important**
this shows how to use promise functions 

![[Pasted image 20250526125243.png]]



this is used to catch all the rejects
![[Pasted image 20250526125628.png]]

