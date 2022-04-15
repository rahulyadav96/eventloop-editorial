# <center> JavaScript Event Loop

JavaScript is a single-threaded programming languages. In other words, it can do only one thing at a time. 

There are four important things works to excute javascript code

1. Memory Heap
2. call stack

3. WebAPIs
    <ul>
        <li> DOM </li>
        <li> AJAX (XMLHttpRequest)</li>
        <li> setTimeout</li>
    </ul>

4. Callback queue


### Memory Heap

    It store data randomly and allocate memmory.


### Call Stack
    Call stack is a function which keeps track of all other functions executed in run time.

    Function get popped out of the stack after a function's purpose gets over.

### Web APIs 
     Since the 'setTimeout' function is part of the Web API, it gets moved to the Web API.
     Ideally, you would have anticipated that the function is returned to the Call Stack for execution. Howevver, instead, it adds it to the Callback queue.

### Call back queue
    Event queue is a data structure similr to stack which holds the data temporarily and the important thing to note is that the data added first is processed first.

### Event Loop

Event loop does the following:

    Checks if the call stack is empty, i.e., if all the functions have completed their execution and they have been off the  call stack.

    Once the call stack is empty, it moves the first item from the Event Queue to the call stack.


Note: The function of Event loop can simply be explain as connecting the callback queue to the callstack.





