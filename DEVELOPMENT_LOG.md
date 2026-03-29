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

### Entry 1 - [March 27, 2026, 6:00 PM]
**What I did**: Reviewed the starter code and set up the project

**Details**: 
- Opened and explored the provided scheduler simulation code
- Ran the program to understand how it works
- Located the section to update the student ID and modified it
- Verified that the program runs correctly before making changes

**Challenges**: Understanding how the existing code is structured, especially the relationship between threads and processes

**Solution**: Carefully read through the code and followed the execution flow step by step

**Time spent**: 45 minutes
---

## Entry 2 - [March 27, 2026, 8:00 PM]
What I did:
Added priority feature to processes

Details:
- Added priority attribute to Process class
- Generated random priority (1–5)
- Displayed priority when adding process to ready queue

Challenges:
- Making sure priority is correctly passed to constructor

Solution:
- Updated constructor and verified output

Time spent:
1.5 hours

---

## Entry 3 - [March 28, 2026, 5:30 PM]
What I did:
Implemented context switch counter

Details:
- Created static variable for context switches
- Incremented it whenever a process starts execution
- Displayed total context switches at the end

Challenges:
- Finding the correct place to increment the counter

Solution:
- Placed it before starting each thread

Time spent:
1 hour 

---

## Entry 4 - [March 28, 2026, 7:00 PM]

**What I did:**
Debugged and fixed an issue in the scheduling loop

**Details:**
- Observed unexpected behavior during process execution
- Reviewed how threads are created and executed in the loop
- Tracked the execution flow to identify the problem

**Challenges:**
- Program crashed due to incorrect thread handling

**Solution:**
- Adjusted the code to ensure each thread is executed correctly without duplication

**Time spent:**
1 hour 

---

## Entry 5 - [March 29, 2026, 6:30 PM]

**What I did:**
Implemented waiting time calculation from scratch

**Details:**
- Added new variables in the Process class to track waiting time
- Created logic to record when a process enters the ready queue
- Updated the code to calculate total waiting time before execution
- Displayed waiting time for each process at the end of the simulation

**Challenges:**
- Figuring out how to correctly track waiting time across multiple executions

**Solution:**
- Used timestamps to measure how long the process stays in the queue before each run

**Time spent:**
2 hours

---

### Entry 6 - [Optional - Date and Time]
**What I did**: 

**Details**: 

**Challenges**: 

**Solution**: 

**Time spent**: 

---

## Summary

**Total time spent on assignment**: [X hours]

**Most challenging part**: 

**Most interesting learning**: 

**What I would do differently next time**: 
