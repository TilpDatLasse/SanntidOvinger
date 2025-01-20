Exercise 1 - Theory questions
-----------------------------

### Concepts

What is the difference between *concurrency* and *parallelism*?
> true parallelism requires multiple cores. Concurrency includes parallelism but can also be achieved with only one core, by switching forth and back between tasks.

What is the difference between a *race condition* and a *data race*? 
> data race is a type of race condition where memory access is not synchronised
 
*Very* roughly - what does a *scheduler* do, and how does it do it?
> The boss, decides which part of the code gets to run at different times.


### Engineering

Why would we use multiple threads? What kinds of problems do threads solve?
> threads enable concurrency and are very helpful for organizing shared memory.

Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they, and why would we rather use them over threads?
> fibers pause and resume without the scheduler controlling them. Less overhead than threads.

Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
> Depends on the situation. If we want different parts of a system to cooperate (eks. shared memory) it is a nice option. In programs where concurrency is not necessary, it is ofcourse easier not to implement it.

What do you think is best - *shared variables* or *message passing*?
> In our case message passing might be the better choice, since safety is important and efficiency (a lot of data) is probably not.


