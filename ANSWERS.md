# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

A process is an independent program in execution that has its own memory space, resources, and execution context. A thread is a smaller unit of execution that runs within a process and shares the same memory and resources with other threads in that process. Threads are lightweight compared to processes because creating a new thread requires less overhead than creating a whole process. In this assignment, we used threads instead of separate processes because all simulated processes needed to access shared structures like the ready queue, and threads can easily share memory. Additionally, threads allow faster context switching and lower creation overhead, which is important when simulating many processes in Round-Robin scheduling.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

In Round-Robin scheduling, if a process doesn’t finish within its allocated time quantum, it is re-queued at the end of the ready queue to wait for its next turn. This ensures that every process gets a fair chance to execute while preventing any single process from monopolizing the CPU.

Example from my output:

  ⏸ P3 completed quantum 2000ms │ Overall progress: [██████░░░░░░░░] 60%
  ↻ P3 yields CPU for context switch
➕ P3 (Priority: 2) added to ready queue | Burst: 5000ms

Explanation of example:
In this snippet, process P3 ran for its time quantum of 2000ms but still has 3000ms remaining. Therefore, it is added back to the ready queue (addProcessToQueue) to be executed in the next round. This re-queueing behavior is important because it maintains fairness, allowing other processes in the queue to run and ensuring that the CPU is shared predictably among all tasks.

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

In the simulation, a thread goes through several states during execution. Here’s the lifecycle for process P1:
1. **New**: When Thread t = new Thread(process); is created, P1 is in the New state because it has been instantiated but has not started running.

2. **Runnable**:After calling t.start(), the thread enters the Runnable state. It is ready to run and waiting for the CPU scheduler to allocate time.

3. **Running**: When the CPU executes P1’s run() method, the thread enters the Running state. Here, it simulates execution for its time quantum using Thread.sleep() for progress steps.

4. **Waiting**:During Thread.sleep(stepTime), P1 temporarily enters a Waiting state. It is paused for the duration of the sleep interval, simulating the passage of execution time.

5. **Terminated**: Once remainingTime <= 0 and the run() method finishes, P1 enters the Terminated state. The thread is no longer alive, and its execution is complete.

This lifecycle is controlled in the code through Thread.start(), Thread.sleep(), and Thread.join(), demonstrating all key thread states in practice.

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: Web Browser

**Description**: 
the browser, allthreadSeparate for handling
**Why Round-Robin works well here**: 
Round-Robin  FatBefore moving on tobrowsing experienceSo that each tab responds
### Example 2:Smartphone apps (such as Whatsapp or Twitter)
**Description**: 
mobile applications, hereAlways. K
**Why Round-Robin works well here**: 
Round-Robin ensures that every mA fair share of the processor , so the application
---

## Summary

**Key concepts I understood through these questions:**
1. Round-Robin scheduling distributes CPU time fairly among all tasks, ensuring fast responsiveness and preventing any single task from monopolizing the CPU.
2. Threads allow multiple tasks to run simultaneously within the same application or system without blocking each other.
3. Re-queueing incomplete tasks ensures fairness and allows all tasks to complete in a balanced way.

**Concepts I need to study more:**
1.Optimizing performance for applications with multiple concurrent tasks and better CPU management in complex scenarios. 
2. Handling thread synchronization and deadlock issues when multiple threads access shared resources.
