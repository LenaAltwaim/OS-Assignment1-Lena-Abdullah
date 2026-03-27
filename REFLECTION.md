# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer: I learned how to build and manage threads using Java's Runnable interface from this assignment.
I discovered that many threads can mimic concurrent execution even if they share the same memory.
CPU. I also learned about the states of the thread lifecycle, such as New, Runnable, Running, and Terminated. One important concept that I understood is how Thread.start() starts execution and Thread. Join() ensures synchronization.

Additionally, scheduling methods like Round-Robin made me aware of the fair distribution of CPU time among threads.
This task helped me draw the dots between textbook theory and real-world application.**

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:The hardest aspect was figuring out how the scheduler works with the queue and threads. The mechanism of re-adding processes to the queue after partial execution was first unclear. Correctly implementing the waiting time feature presented another difficulty since it necessitated an understanding of how time is tracked in actual systems. It was also challenging to decide where to make code changes without altering the original reasoning. The situation becomes more complicated due to the interplay between threads and time.
In general, it required both conceptual knowledge and code.**

[Describe the specific challenge. Was it understanding the code? Implementing a feature? Using Git? Explain what made it difficult and how it relates to the course concepts.]

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:By carefully reviewing the code several times and connecting it to ideas from the Operating Systems textbook, I was able to overcome these difficulties. After every change, I also regularly checked the program to make sure it was accurate. I was able to concentrate on one aspect at a time by breaking the task down into smaller pieces.
In order to comprehend program behavior, I also employed debugging strategies such printing intermediate values. My comprehension was further strengthened by watching multithreading tutorials. I grew more comfortable changing the code over time.**

[Describe your problem-solving approach. Did you read documentation? Ask for help? Debug systematically? What resources did you use? What strategies worked?]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:Real-world applications like web browsers, where each tab operates as an independent thread, frequently use multithreading. Additionally, servers use it to manage several client requests at once. Threads are used in games to concurrently handle physics, graphics, and user input. Threads are used by media players to manage user controls and play music and video. I gained a better understanding of how threads increase efficiency and responsiveness thanks to this project. Additionally, it demonstrated how scheduling guarantees equitable resource distribution.**

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?
-----
[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?

[Rate yourself and explain: Beginner / Intermediate / Confident]
I'm rating myself Beginner/Intermediate

[Explain your rating - what do you understand well? What needs more practice?]
 I understand the basic concepts such as thread creation, lifecycle, and scheduling, but I still need more practice with complex synchronization problems and real-world systems.
---

### Feedback on the assignment
 very helpful in understanding multithreading concepts practically, It was challenging but also rewarding because it connected theory with real implementation. tho more examples or hints could make it easier for beginners.
[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
