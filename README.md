# ☕ Java Multithreading & Concurrency

**A structured, beginner-friendly guide to Java multithreading, concurrency, and asynchronous programming.**

This repository helps developers understand how Java handles multiple tasks, manages threads, protects shared resources, and executes asynchronous operations through practical examples.

## 📌 Table of Contents

1. [Overview](#-overview)
2. [Learning Objectives](#-learning-objectives)
3. [Core Concepts](#-core-concepts)
4. [Multithreading vs Concurrency vs Parallelism](#-multithreading-vs-concurrency-vs-parallelism)
5. [Java Concurrency Tools](#-java-concurrency-tools)
6. [Real-World Applications](#-real-world-applications)
7. [Prerequisites](#-prerequisites)
8. [Getting Started](#-getting-started)
9. [Recommended Learning Path](#-recommended-learning-path)
10. [Author](#-author)

---

## 🎯 Overview

Multithreading is a programming technique that allows multiple threads to execute within a single application.

It is widely used in backend development, background processing, concurrent request handling, and other applications where multiple tasks need to make progress efficiently.

This repository focuses on understanding the concepts step by step, from creating a basic thread to managing concurrent tasks with Java's concurrency APIs.

## 🎓 Learning Objectives

By studying this repository, you will learn how to:

- Create and execute threads in Java.
- Understand thread lifecycle and scheduling.
- Execute multiple tasks concurrently.
- Identify and prevent race conditions.
- Synchronize access to shared resources.
- Manage tasks using thread pools.
- Handle asynchronous results and exceptions.
- Understand common concurrency problems such as deadlocks.
- Apply concurrency concepts to backend applications.

---

## 🧠 Core Concepts

### 1. Thread Fundamentals

| Concept | Explanation |
|---|---|
| Thread | An independent path of execution within a process |
| `Thread` | Java class used to create and manage a thread |
| `Runnable` | Represents a task that can be executed by a thread |
| Thread Lifecycle | Describes the states a thread can occupy |
| `start()` vs `run()` | `start()` initiates a new thread; calling `run()` directly executes it like a normal method |

### 2. Concurrency and Parallelism

- **Concurrency:** Multiple tasks make progress over overlapping periods.
- **Parallelism:** Multiple tasks execute simultaneously, typically on different CPU cores.
- **Context Switching:** The operating system or runtime switches execution between threads.
- **Thread Scheduling:** Determines when threads get execution time.

### 3. Synchronization and Thread Safety

| Concept | Purpose |
|---|---|
| Race Condition | Occurs when concurrent operations produce incorrect results due to timing |
| `synchronized` | Coordinates access to protected code or shared state |
| `volatile` | Provides visibility guarantees for a variable between threads |
| `Lock` | Provides explicit locking mechanisms |
| Atomic Classes | Support thread-safe atomic operations |
| Deadlock | Threads wait indefinitely for resources held by one another |

### 4. Thread Management

- `ExecutorService` — executes and manages submitted tasks.
- Thread Pools — reuse worker threads to reduce thread-creation overhead.
- `Callable` — represents a task that returns a result and can throw checked exceptions.
- `Future` — represents a result that may become available later.
- `ScheduledExecutorService` — executes tasks after delays or periodically.

### 5. Asynchronous Programming

- `CompletableFuture` — composes asynchronous computations.
- `thenApply()` — transforms a successful result.
- `thenCompose()` — chains asynchronous operations that return another `CompletionStage`.
- `thenCombine()` — combines results from independent computations.
- `exceptionally()` — provides a way to recover from certain failures.
- `allOf()` — waits for multiple futures to complete.

---

## ⚖️ Multithreading vs Concurrency vs Parallelism

| Feature | Meaning |
|---|---|
| Multithreading | Using multiple threads in one application |
| Concurrency | Managing multiple tasks that overlap in progress |
| Parallelism | Executing multiple tasks at the same time |
| Asynchronous Programming | Allowing work to proceed without synchronously waiting for its result |

These concepts are related, but they are not interchangeable. A multithreaded application may be concurrent without executing all tasks in parallel.

---

## 🛠️ Java Concurrency Tools

The following Java APIs are useful for implementing concurrent applications.

| API | Common Use Case |
|---|---|
| `Thread` | Basic thread execution |
| `Runnable` | Tasks without a return value |
| `Callable` | Tasks that return a result |
| `ExecutorService` | Managing task execution |
| `Future` | Retrieving results from submitted tasks |
| `CompletableFuture` | Composing asynchronous operations |
| `CountDownLatch` | Waiting for a set of operations to complete |
| `Semaphore` | Limiting concurrent access to a resource |
| `ReentrantLock` | Explicit mutual exclusion |
| `AtomicInteger` | Atomic integer updates |

---

## 🌍 Real-World Applications

### Backend Development

Handle multiple client requests and execute independent background tasks efficiently.

### E-Commerce

Process independent activities such as notifications, reporting, and inventory-related tasks while maintaining data consistency.

### File Processing

Process independent files concurrently when the workload and available resources make it beneficial.

### External API Integration

Call independent services asynchronously and combine their results when appropriate.

### Scheduled Jobs

Execute recurring tasks such as periodic cleanup, reporting, and status checks.

**Important:** Multithreading does not automatically make every operation faster. Performance depends on the workload, available resources, and correct concurrency design.

---

## 💻 Prerequisites

Before running the examples, make sure you have:

- Java Development Kit (JDK) installed.
- Git installed.
- IntelliJ IDEA, Eclipse, or another Java IDE.
- Basic knowledge of Java classes, methods, and object-oriented programming.

---

## 🚀 Getting Started

### Step 1: Clone the Repository

```bash
git clone https://github.com/istiakahasan/Multi-Threading.git
```

### Step 2: Open the Project

Open the cloned folder in your Java IDE.

### Step 3: Run an Example

1. Locate a Java class containing a `main()` method.
2. Read the code and identify the task being executed.
3. Run the class.
4. Observe the output.
5. Run it multiple times to see how concurrent execution can affect output ordering.

### Step 4: Experiment

Modify the examples to understand the behavior of threads, synchronization, and task execution.

---

## 🗺️ Recommended Learning Path

Follow this order to build your understanding progressively.

1. **Beginner:** `Thread`, `Runnable`, `start()`, and thread lifecycle.
2. **Intermediate:** Race conditions, synchronization, and thread safety.
3. **Task Management:** `ExecutorService`, thread pools, `Callable`, and `Future`.
4. **Concurrency Utilities:** Locks, atomic variables, latches, and semaphores.
5. **Asynchronous Programming:** `CompletableFuture` and exception handling.
6. **Advanced:** Deadlocks, producer-consumer patterns, performance considerations, and virtual threads.

---

## 📚 Key Takeaways

- Threads allow tasks to execute independently.
- Concurrency requires careful management of shared state.
- Synchronization helps prevent certain race conditions.
- Thread pools provide controlled task execution.
- Asynchronous programming helps compose operations without synchronous waiting.
- Correctness and maintainability matter as much as performance.

---

## 👨‍💻 Author

**Istiak Ahasan**

Java Backend Developer | Spring Boot Developer | AI Enthusiast

- GitHub: [@istiakahasan](https://github.com/istiakahasan)
- Repository: [Java Multithreading](https://github.com/istiakahasan/Multi-Threading)

---

⭐ If you find this repository helpful, consider giving it a star.

**Learn the concepts. Practice with code. Build reliable concurrent applications.**
