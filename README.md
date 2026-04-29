# E-Portfolio – Iley Demir

## About Me
I am a second-year Information and Communication Technology student at KTH with an interest in software development and embedded systems, with a long-term interest in AI and cybersecurity. Through my coursework, I have gained experience in networking, low-level programming, and algorithm analysis.

---

## Projects

### Concurrent HTTP Server with TCP Client Integration (Java)
- Implemented a multi-threaded HTTP server capable of handling multiple client connections concurrently
- Parsed HTTP/1.1 GET requests and validated request structure
- Extracted and processed query parameters (hostname, port, string, timeout, limit)
- Integrated a custom TCP client to communicate with external servers and return responses
- Implemented proper HTTP responses including status codes (200, 400, 404)

**My contribution:**
- Independently designed and implemented all components of the system
- Built concurrent client handling using threads
- Implemented full HTTP request parsing and validation logic
- Developed TCP client functionality with support for timeout, shutdown, and response limits

**Technologies:** Java, TCP/IP, HTTP, Multithreading

**Example snippet:**
```java
String[] parts = requestLine.split(" ");
if (!parts[0].equals("GET") || !parts[2].equals("HTTP/1.1")) {
    send400(output);
}
```

**Note:** Full implementation is not publicly available due to academic integrity policies.

---

### Computer Hardware Engineering Lab – Interrupt Handling
- Implemented timer-driven functionality using low-level hardware registers
- Worked with direct memory access and bitwise operations for hardware interaction
- Developed functionality for handling input from buttons and switches and updating display output

**My contribution:**
- Implemented timer configuration and polling logic
- Handled hardware status flags and control registers
- Developed logic for real-time updates and user input handling

**Technologies:** C, microcontrollers

**Example snippet:**
```c
volatile unsigned int *timer = (volatile unsigned int *)0x04000020;
unsigned int status = timer[0];

if (status & 0x1) {
    timer[0] = 0; // clear timeout flag
}
```

**Note:** Full implementation is not publicly available due to academic integrity policies.

---

### Search Algorithms and Complexity Analysis (C)
- Implemented and compared linear search and binary search on arrays
- Evaluated performance differences between unsorted and sorted data
- Measured execution time across varying input sizes to analyze scalability
- Compared iterative and recursive approaches for binary search

**My contribution:**
- Independently implemented all algorithms in C
- Conducted benchmarking and performance analysis
- Interpreted results to determine time complexity behavior

**Technologies:** C, Algorithm Analysis

**Example snippet:**
```c
int index = (first + last) / 2;
if (array[index] == key) {
    return true;
}
```

**Key insights:**
- Linear search has O(n) time complexity and scales linearly with input size  
- Binary search has O(log n) time complexity and remains efficient for large datasets  

**Note:** Full implementation and report are not publicly available due to academic integrity policies.

---

## Skills

- Programming: Java, C  
- Tools: Git, VS Code  
- Concepts: Networking (TCP/IP, HTTP), Embedded Systems, Algorithm Analysis  

---

## Additional Information
Some project details and code are limited due to academic integrity policies. Further information can be provided upon request.
