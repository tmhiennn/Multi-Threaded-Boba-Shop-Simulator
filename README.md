# BobaQueue: Order Management & Printing Simulator

A Java-based Point of Sale (POS) simulation that manages a boba shop's workflow. The program handles randomized customer traffic, manages order queues, and simulates a copier printing receipts with specific hardware constraints.

## 🚀 Features
- **Order Queuing:** Uses a Queue data structure to manage high volumes of incoming orders.
- **Hardware Simulation:** Simulates a copier that processes print jobs in 10-page increments.
- **Automated Wait-Time Logic:** Calculates estimated pickup times dynamically based on the number of workers available.
- **Reporting:** Includes a "Summary of the Day" feature displaying top-selling drinks, total income, and worker performance.
- **Data Sorting:** Implements **QuickSort** to organize customer information for end-of-day records.

## 🛠️ How it Works (Algorithm)
1. **Initialize:** Loads menu items and customer names from text files using `BufferedReader`.
2. **Simulation:** Generates a random number of orders and workers for the day.
3. **Queue Management:** Orders are assigned to specific queues using the `determineQueueIndex` method.
4. **Processing:** Each order is processed into a `PrintOrder` job.
5. **Output:** Receipts are printed with time estimates and payment methods (Cash/Card).
6. **Summary:** Displays a final analytics report of the shop's performance.

## 💻 Technical Stack
- **Language:** Java
- **Data Structures:** ArrayList, Queue, Arrays
- **Algorithms:** QuickSort, Randomized Simulation
- **File I/O:** BufferedReader

## 📄 Sample Receipt Output
```text
----------------------------
      BOBA SHOP RECEIPT
----------------------------
Order No: 5
Customer: Hien Tran
Drink: Classic Milk Tea
Total Cups: 2
Payment: Card
Est. Wait Time: 4 mins
----------------------------
