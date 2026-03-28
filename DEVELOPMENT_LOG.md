# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

Entry 1 - [Mar 27, 2026, 11:23 PM]

What I did: Signed in GitHub and set up the repository and project

Details:

Logged into GitHub
Opened the assignment repository and created my own copy
Reviewed project files and structure
Opened the project locally and prepared environment for coding

Challenges:
Was unsure how the project files were organized and which file to start with

Solution:
Read the instructor guide and explored each file to understand the workflow

Time spent: 1 hour
---

#Entry 2 - [Mar 28, 2026, 12:30 AM]

What I did: Implemented Feature 1 (Priority Scheduling)

Details:

Added a priority attribute to the Process class
Used Random to assign priority values (1–5)
Created a getter method getPriority()
Displayed priority when processes are added to the queue

Challenges:
Was unsure how to integrate priority without breaking the existing Round Robin logic

Solution:
Kept Round Robin scheduling unchanged and added priority as an additional attribute for display only

Time spent: 35 minutes

---

Entry 3 - [Mar 28, 2026, 1:15 AM]

What I did: Implemented Feature 2 (Context Switch Counter)

Details:

Added a static variable contextSwitchCount in SchedulerSimulation
Incremented it every time a new process is scheduled (poll() from queue)
Displayed total context switches at the end of execution

Challenges:
Did not initially know where exactly to count context switches

Solution:
Placed the counter increment inside the scheduling loop where each process gets CPU time

Time spent: 25 minutes
---

Entry 4 - [Mar 28, 2026, 1:45 AM]

What I did: Implemented Feature 3 (Waiting Time Tracking)

Details:

Added creationTime and waitingTime variables
Recorded creation time using System.currentTimeMillis()
Calculated waiting time after each execution
Displayed waiting time in the final summary

Challenges:
Understanding how to correctly calculate waiting time in a multi-threaded simulation

Solution:
Used system time difference (current time – creation time) as an approximation

Time spent: 40 minutes
---

Entry 5 - [Mar 28, 2026, 2:20 AM]

What I did: Worked on the ANSWERS.md file

Details:

Opened and edited the ANSWERS.md file in GitHub
Answered all required assignment questions
Ensured answers were clear and properly formatted
Used ChatGPT to better understand some concepts before writing answers

Challenges:
Some questions were unclear and required deeper understanding of scheduling concepts

Solution:
Reviewed course material and used external help to simplify the concepts before writing them in my own words

Time spent: 40 minutes
---

Entry 6 - [Mar 28, 2026, 2:45 AM]

What I did: Completed the REFLECTION.md file and final review

Details:

Edited REFLECTION.md and wrote about what I learned from the assignment
Reflected on challenges faced during implementation
Reviewed all files (code, answers, and log) to ensure completeness
Made final formatting corrections

Challenges:
It was difficult to clearly express what I learned and summarize the experience

Solution:
Focused on key concepts (Round Robin, context switching, waiting time) and wrote simple, clear points

Time spent: 30 minutes
---

## Summary

**Total time spent on assignment**: [~5-6 hours 20 minutes] (seperated in 2 days)

**Most challenging part**: Correctly implementing the waiting time and knowing where to track context transitions in the scheduling loop proved to be the most difficult aspects. Additionally, it took some time to properly comprehend the practical operation of round robin scheduling.

**Most interesting learning**: was using simulation to observe how CPU scheduling operates. I was able to gain a better understanding of issues like fairness, context switching, and process waiting time by implementing processes as threads and observing their execution with time quantum.

**What I would do differently next time**: Rather of recreating my work afterward, I would begin documenting it right now. In order to identify problems early, I would also test every feature as soon as it was implemented.
