# Lab 2
## Exercise 1
1. List the four conditions that need to be satisfied for a deadlock to occur.
* Mutual exclusion: only one process at a time can use a resource.
* Hold and wait: a process holding at least one resource is waiting to acquire additional resources held by other processes.
* No preemption: a resource can be released only voluntarily by the process holding it.
* Circular wait: there exists a set {P0, P1, …, Pn} of waiting processes such that P0 is waiting for a resource that is held by P1, P1 is waiting for a resource that is held by P2, …, Pn–1 is waiting for a resource that is held by Pn, and Pn is waiting for a resource that is held by P0.

2. Which of the four deadlock conditions did
   you attempt at breaking? How does your
   solution break that deadlock condition?
* Hold and wait: a philosopher will wait for his first fork and then try to acquire the second one. If he can't acquire the second one, he will release the first one and try again. This way, he will not hold any fork while waiting for the second one.
3. Try to give short descriptions of solutions which attacks the three other deadlock criteria.
* Mutual exclusion: the forks are shared resources, so they can be used by multiple philosophers at the same time.
* No preemption: another philosopher can take the fork from a philosopher who is waiting for the second fork.
* Circular wait: the philosophers will not try to acquire the forks in the same order, so there will be no circular wait.