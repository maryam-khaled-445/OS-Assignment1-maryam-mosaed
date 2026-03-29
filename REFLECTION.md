# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:**
 
From this assignment, I learned how multithreading allows multiple threads to run concurrently, simulating parallel execution. I explored thread creation in Java using the `Runnable` interface and `Thread` class, and observed how threads have different states such as running, waiting, and terminated. It was interesting to see how context switching occurs between threads in the scheduler. I also learned that threads can share resources, which requires careful tracking to avoid conflicts. Implementing the CPU scheduler made me realize the importance of synchronizing access to shared data like waiting time. Overall, I now understand how threads can improve efficiency by performing tasks seemingly at the same time. The assignment also showed me the practical difference between thread execution order and scheduling logic.
---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:**
The most challenging part of this assignment was managing synchronization between multiple threads. At first, it was difficult to understand how shared resources could be accessed safely without causing race conditions or inconsistent results. For example, when I tried updating a shared counter from two threads simultaneously, the final output was sometimes incorrect, which was confusing. Understanding the need for locks or synchronized blocks was essential but took some trial and error. Additionally, keeping track of which thread was running and debugging thread interleaving issues was tricky. I also struggled with visualizing the execution order, as threads don’t run linearly. Overall, figuring out how to control thread access while still allowing parallel execution was the most challenging aspect.




---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:**

I overcame these challenges mainly by watching YouTube tutorials on Java multithreading, which provided clear examples of creating threads, using synchronized blocks, and avoiding race conditions. The videos helped me visualize how threads run concurrently and how shared resources can be accessed safely. I followed along with some example code and adapted it to my own assignment, which made it easier to understand the concepts in practice. Additionally, I used print statements to monitor thread execution and check if my changes were working correctly. Step by step, I implemented synchronization mechanisms and tested each modification until the threads behaved as expected. Using this combination of video guidance and hands-on experimentation allowed me to overcome the difficulties and learn multithreading effectively.
---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**

Multithreading is widely used in real-world applications to make programs more efficient and responsive. For example, web browsers use multiple threads to load images, scripts, and content simultaneously, so the page does not freeze while waiting for network responses. Mobile apps often use threads to perform background tasks, like downloading data or processing images, without blocking the user interface. Games also use threads for tasks such as rendering graphics, handling AI, and managing player input at the same time. From this assignment, I learned how threads allow simultaneous execution, which reduces waiting time and improves performance. I now understand that careful thread management and synchronization are crucial to avoid errors and ensure smooth operation in these scenarios.

---

## Additional Reflections (Optional)

### What would you like to learn more about?

I would like to learn more about advanced concurrency concepts, such as thread pools, semaphores, and concurrent data structures. I am also curious about deadlocks and thread priorities, and how professional applications manage multiple threads efficiently. Watching YouTube tutorials gave me a good introduction, but I want to explore these topics further to understand how multithreading is applied in large-scale real-world systems like web servers and multiplayer games.

---

### How confident do you feel about multithreading concepts now?

I would rate myself as Intermediate. I now understand the basics of creating threads, running them concurrently, and using synchronization to protect shared resources. However, I need more practice with complex issues like avoiding deadlocks, optimizing thread performance, and using advanced concurrency tools. The YouTube tutorials helped me gain confidence in applying what I learned to my assignment, but I know I need more hands-on practice to become fully confident.

---

### Feedback on the assignment

This assignment was very helpful because it allowed me to practice multithreading in a real coding scenario rather than just reading theory. Some parts were challenging, especially debugging concurrent threads, but using video tutorials made it much easier to understand. It would be helpful if future assignments included v or more examples of real-world applications, which could make it even easier to grasp thread behavior. Overall, it was a great learning experience.
