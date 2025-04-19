# Java Multi-threading Application

## 📌 Overview

This Java application demonstrates the use of **multi-threading** by implementing the `Runnable` interface. It creates and starts multiple threads that perform numerical operations in parallel with specified delays.

---

## 🧱 Project Structure

---

## 🚀 How It Works

### ✅ `Main.java`
- Acts as the **entry point** of the program.
- Creates two threads using the `MyThread` class:
  - `Thread t1`: Starts from 1, increments by 3, sleeps 3 seconds
  - `Thread t2`: Starts from 100, increments by 50, sleeps 1 second
- Threads are started using `.start()` to run concurrently.

### ✅ `MyThreads.java`
- Implements `Runnable` to define the **thread behavior**.
- Accepts:
  - `init` — initial value
  - `increment` — value to increase each time
  - `delay` — delay between iterations (in milliseconds)
- Inside `run()`:
  - Prints the current value
  - Increments it
  - Pauses the thread using `Thread.sleep(delay)`
  - Stops if value reaches/exceeds 1000

---

## 🛠 Technologies Used

- Java
- Multi-threading (`Runnable`, `Thread`, `sleep()`)

---

## 💡 Use Case

Ideal for understanding how threads run independently, how delays affect thread execution, and how concurrent output behaves in the console.

---

## 📝 How to Run

1. Compile both `.java` files:
   ```bash
   javac MyThreads.java Main.java

