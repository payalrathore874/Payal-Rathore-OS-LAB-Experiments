# Operating System Assignments

**Name:** Payal Rathore  
**Roll No.:** 2301410022  
**Course:** BTech CSE (Cyber Security)

---

## 📌 Linux Process Simulation

This repository contains assignments that simulate core operating system concepts using Python.

---

## **Assignment 1: Linux Process Management**

### Tasks
1. **Create processes** using `os.fork()`.  
2. **Execute system commands** with `os.execvp()`.  
3. **Demonstrate** zombie and orphan processes.  
4. **Inspect process details** from `/proc/[pid]`.  
5. **Assign process priorities** using `os.nice()`.  

---

## **Assignment 2: System Startup Simulation**

- Simulates a simplified system startup using the `multiprocessing` and `logging` modules.  
- Creates multiple child processes, runs dummy tasks, and logs lifecycle events.  
- Generates a log file: **`process_log.txt`**.  

---

## **Assignment 3: Scheduling**

Implements **CPU scheduling algorithms** in Python.

### Algorithms Implemented
- **First Come First Serve (FCFS):** Processes are scheduled in the order they arrive.  
- **Shortest Job First (SJF):** Process with the shortest burst time is scheduled first.  
- **Round Robin (RR):** Each process gets a fixed time quantum in cyclic order.  

### Metrics Calculated
- **Waiting Time**  
- **Turnaround Time**  
- **Average Waiting Time**  
- **Average Turnaround Time**  

### Comparison
- **SJF:** Gives the lowest average waiting and turnaround time, but may cause starvation of long processes.  
- **FCFS:** Simple but can lead to the convoy effect if a long job arrives first.  
- **Round Robin:** Ensures fairness (all processes get CPU time), but performance depends on the time quantum chosen.

  ## Assignment 3: Memory Allocation Strategies

Simulates different memory allocation strategies in an operating system.

### Algorithms Implemented
- **First Fit:** Allocates the first block that is large enough for the process.
- **Best Fit:** Allocates the smallest block that is large enough to minimize waste.
- **Worst Fit:** Allocates the largest available block to reduce future fragmentation.

### Metrics Observed
- Process allocation success or failure.
- Block utilization after allocation.

### How to Run
```bash
python3 memory_allocation.py


---

## ⚙️ Tools Used
- **Python 3.x**  
- Modules: `os`, `subprocess`, `multiprocessing`, `time`, `logging`  

---

## 🚀 How to Run

```bash
# Assignment 1: Linux Process Management
python3 process_management.py

# Assignment 2: System Startup Simulation
python3 startup_simulation.py
cat process_log.txt   # View generated log file

# Assignment 3: Scheduling

# Run First Come First Serve
python3 fcfs.py

# Run Shortest Job First
python3 sjf.py

# Run Round Robin (with user-defined quantum)
python3 round_robin.py
