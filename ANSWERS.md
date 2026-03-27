# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:A thread is a smaller unit of execution within a process that shares memory, whereas a process is an independent program in execution with its own memory space. Threads are lighter and quicker to construct than processes, which are heavier and need more resources to build and manage.
Compared to processes, threads facilitate faster and easier communication because they share memory. Because threads enable effective simulation of several processes within a single program, they were used in this project. More overhead and intricate communication methods would be needed if distinct procedures were used.**

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer: Round-Robin scheduling places a process back in the ready queue if it doesn't complete inside its time quantum. This guarantees that each process receives an equal amount of CPU time. Because every process has an equal chance to be carried out, this behavior guarantees justice and eliminates famine. .**

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output: 
P2 executing quantum [4000ms]
  ⚡ Quantum progress: [███████████████] 100%
  ⏸ P2 completed quantum 4000ms │ Overall progress: [█████████░░░░░░░░░░░] 45%
     Remaining time: 4726ms
  ↻ P2 yields CPU for context switch

  ➕ P2 added to ready queue │ Burst time: 8726ms | Priority: 1
```
```

**Explanation of example:**
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1 New:
P1 is in the New state when it is first created at the start of the simulation. This happens before it is added to the ready queue (when the program initializes all processes).

2 Runnable:
P1 becomes Runnable when it is added to the ready queue:
➕ P1 added to ready queue │ Burst time: 3919ms

At this point, P1 is ready to execute but is waiting for the CPU.

3 Running:
P1 enters the Running state when the scheduler selects it and assigns the CPU:
▶ P1 executing quantum [3919ms]

Here, P1 is actively using the CPU.

4 Waiting:
In this simulation, P1 does not enter the Waiting state.
Waiting usually happens if a process is blocked (e.g., waiting for I/O).
Your simulation is CPU-bound (Round Robin scheduling), so processes only move between Runnable ↔ Running, not Waiting.

5 Terminated:
P1 enters the Terminated state after finishing execution:
✓ P1 finished execution!
Its remaining time becomes 0ms
It is removed from the system and does not return to the queue

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer: 
example 1: Web server
Description: A web server uses threads to manage several client requests at once.
Why Round-Robin is effective in this situation: By allocating a tiny time slice to each request, Round-Robin guarantees fairness. This enhances responsiveness and keeps additional requests from being blocked by a single request.

Example 2: Task Scheduling in the Operating System
CPU scheduling techniques are used by an operating system to schedule several running applications.
Why Round-Robin is effective in this situation: It guarantees that CPU time is distributed fairly among all processes. Additionally, it enhances system responsiveness, particularly for interactive applications.

**

---

## Summary

**Key concepts I understood through these questions:**
1. The distinction between processes and threads
2. Round-Robin scheduling behavior
3. Lifecycle of a thread

**Concepts I need to study more:**
1. Synchronization of threads
2. Advanced scheduling algorithms
