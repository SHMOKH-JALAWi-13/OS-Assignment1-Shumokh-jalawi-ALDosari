# Assignment 1 - Work Summary

- **Student ID:** 445052013
- **Student Name:** Shumookh AlDosari
- **Repository:** https://github.com/SHMOKH-JALAWI-13/OS-Assignment1-Shumookh-AlDosari

## Development Log
- **2026-10-06:** Forked the starter repository and updated student ID in SchedulerSimulation.java.
- **2026-10-07:** Implemented Process Priority feature (random 1-10) and verified queue display.
- **2026-10-08:** Implemented Context Switch Counter and verified accurate tracking in loops.
- **2026-10-09:** Added simulation statistics tracking for waiting time and turnaround time.
- **2026-10-10:** Finalized code testing, code cleanup, and drafted MY_WORK.md documentation.

## Reflection
1. What was the most challenging part of this assignment and how did you overcome it?
The most challenging part was understanding how the threads interact within the Round-Robin queue and managing the remaining time correctly without breaking the existing simulation structure. I overcame this by carefully reviewing the starter code structure, breaking down the requirements into small steps, and testing each feature incrementally.

2. How did you ensure your output was unique to your student ID?
I made sure to assign my university student ID (445052013) to the random number generator seed in the main method. This ensures that the generated number of processes, time quantum, burst times, and process priorities are uniquely seeded and reproducible based specifically on my student ID.

3. What did you learn about CPU scheduling algorithms from this implementation?
Implementing this simulation gave me a clear, practical understanding of how operating systems handle process scheduling using time slices. I learned how context switching introduces overhead and how processes alternate between running and waiting states in a round-robin queue.

4. How did using Git and GitHub help you structure your assignment workflow?
Using Git and GitHub helped me maintain a clean, organized workflow by breaking the assignment into distinct, meaningful commits for each implemented feature. This practice not only prevented losing progress but also aligned with professional software development standards.

## Technical Answers
1. Difference between a Process and a Thread in Java:
A process represents an independent execution environment with its own memory space and resources, whereas a thread is the smallest unit of execution within a process. In this assignment, each Process object implements Runnable and runs inside its own Thread, allowing multiple execution flows to share the resources of the main simulation program.

2. How the Ready Queue behaves in this Round-Robin simulation:
The Ready Queue operates on a First-In-First-Out (FIFO) basis using a LinkedList queue of threads. When a process exhausts its time quantum and still has remaining execution time, it is re-enqueued at the back of the ready queue, allowing other processes their fair share of CPU time.

3. Explain the Java Thread Lifecycle states observed in your code:
Throughout the simulation, threads transition through multiple states including New (when created via `new Thread()`), Runnable (when added to the queue and started via `currentThread.start()`), Timed Waiting (when executing `Thread.sleep()` during quantum simulation), and Terminated (when the thread finishes execution).

4. Real-world application of CPU scheduling and multithreading:
Modern operating systems rely heavily on CPU scheduling algorithms like Round-Robin to ensure fair CPU allocation and responsive multitasking across multiple running applications and background services. Multithreading allows systems to handle user interfaces, network requests, and heavy computations concurrently without freezing the system.

## Video Demonstration Link
- **Video URL:** [PASTE_YOUR_PUBLIC_VIDEO_LINK_HERE]
