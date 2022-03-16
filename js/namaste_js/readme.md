1. Everything in JS happens inside a `execution context`.
2. `Execution context` consists of : 
  - `Memory component` in JS - `Variable environment`. Variables and function values stored in key-value format.
  - `Code component` in js called - `thread of execution`.
3. Synchronous single-threaded language. 
  - single-threaded : JS can execute only one command at a time. 
  - Synchronous :  execture in a particular order.
4. What happens when we run JS code?
    - Two steps : 
    - 1 : Creation phase
    ![js1](https://user-images.githubusercontent.com/60391776/158552959-4271d175-b24a-4e03-901b-f24d3b90d7d1.png)
    - 2 : Code execution phase : when a function is called, then another `execution context` is created which also has memory and cod 
