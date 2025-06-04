## **JARVIS OS: A Custom Operating System Simulator**  

### **Overview**  
**JARVIS OS** is a **custom operating system simulator** built in **C++** that mimics core OS functionalities such as **process scheduling, memory management, process synchronization, and multilevel queue scheduling**. The project demonstrates how an OS manages multiple tasks efficiently while handling **RAM allocation, priority-based scheduling, and process synchronization** using **mutex locks**.  

This simulator includes **15+ pre-defined tasks** (like Calculator, Tic-Tac-Toe, Banking System, etc.) and allows users to **add, remove, and execute processes dynamically**.  

---

## ** Key Features**  

### **1. Process Scheduling (Priority-Based)**
- **Priority Scheduling Algorithm**: Higher-priority processes execute first.  
- **Context Switching**: Handles process switching efficiently.  
- **Dynamic Process Management**: Users can add or remove tasks at runtime.  

### **2. Memory Management**
- **RAM Allocation & Deallocation**: Tracks RAM usage for each process.  
- **Waiting & Ready Queues**: If RAM is insufficient, processes wait in a queue.  

### **3. Process Synchronization**
- **Mutex Locks**: Ensures thread-safe execution of critical sections.  
- **Process Duplication**: Uses `fork()` to demonstrate process creation.  

### **4. Multilevel Queue Scheduling**
- **Priority-Based Execution**: Processes are grouped into queues based on priority levels.  

### **5. Interactive User & Kernel Modes**
- **User Mode**: Runs pre-defined applications (Calculator, Games, File Handling, etc.).  
- **Kernel Mode (Admin)**: Allows adding/deleting tasks (password-protected).  

---

## ** Technologies Used**  
- **C++** (OOP, Multithreading, System Programming)  
- **POSIX Threads (`pthread`)** for multithreading  
- **Shared Memory (IPC)** for inter-process communication  
- **Linux System Calls (`fork()`, `gnome-terminal` execution)**  

---

## ** How It Works?**  
1. **Initialization**:  
   - The OS loads 15 default tasks with predefined priorities and RAM usage.  
   - Users can log in as **User** (to run apps) or **Kernel** (admin mode).  

2. **User Mode**:  
   - Displays a **menu of applications** (Calculator, Banking System, Games, etc.).  
   - Uses **priority scheduling** to execute tasks.  
   - If RAM is insufficient, processes wait in a **queue**.  

3. **Kernel Mode**:  
   - **Add/Remove Tasks** dynamically.  
   - **Monitor running processes** (Task Manager).  

4. **Process Execution**:  
   - Each task runs in a **separate terminal** using `gnome-terminal`.  
   - **RAM is deallocated** once a process completes.  

---

## **Why This Project?**  
- **Learn OS Concepts**: Deep dive into **scheduling, memory management, and synchronization**.  
- **Hands-on C++ System Programming**: Uses **multithreading, IPC, and Linux system calls**.  
- **Scalable**: Can be extended with **new scheduling algorithms (Round Robin, FCFS)**.  
