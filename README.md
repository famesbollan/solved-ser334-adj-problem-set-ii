Download Link: https://assignmentchef.com/product/solved-ser334-adj-problem-set-ii
<br>
Complete the following four problems. Both the syllabus rules and ADJ Ruleset 1v2 are in e ect.

M7: Process Synchronization I

<ol>

 <li>[Silberschatz, Acuæa] Assume that a context switch takes time <em>T </em>. Propose an algoithm to determine how long a process to hold a spinlock, based on the process load of a system and T. If the spinlock is held for long, switching to a mutex lock (where waiting threads are put to sleep) would give the system better CPU utilization by decreasing wasted cycles (i.e, the busy waiting in a spinlock). Analyze the problem, design an algorithm for computing the bound, and justify the algorithm’s optimality.</li>

</ol>

[5A+3D+5J points]

M9: CPU Scheduling

<ol start="2">

 <li>[Acuæa] Design an e cient (i.e., Big-Oh of a polynomial) algorithm for determining the time quantum t for a round robin scheduler. The algorithm must consider the current process load and compute t, where system throughput is maximized for some interval. Analyze the problem, design an algorithm for computing the bound, and justify the algorithm’s optimality. [5A+3D+5J points]</li>

</ol>

M11: Virtual Memory

<ol start="3">

 <li>[Acuæa] Consider the following fragment of code:</li>

</ol>

#define OFFSET(x , y ,                      columns) = (y ∗ columns + x)

//check i f two matrices are the same . int equals ( IntMatrix∗ this , IntMatrix∗ other ) { i f ( other == NULL) return 0;

i f ( other−&gt;cols != this−&gt;cols | | other−&gt;rowsls != this−&gt;rows) return 0;

for ( int y = 0; y &lt; this−&gt;rows ; y++) for ( int x = 0; x &lt; this−&gt;cols ; x++)

//no intentational magic ; pointer arithmetic since C won’ t allow [ ] [ ] i f (∗( this−&gt;data + OFFSET(x , y , this−&gt;cols )) !=

∗( other−&gt;data + OFFSET(x , y , this−&gt;cols )) return 0;

return      1;

}

What page replacement scheme (of FIFO, OPR, LRU, MFU) should be used for this code? Analyze the problem, design a choice, and justify the choice. [5A+4D+5J points]