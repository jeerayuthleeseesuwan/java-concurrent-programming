# Java Concurrent Programming Project
This Java program simulates a bus terminal scenario. 

## Key concept applied:
1. Multiple threads running concurrently
2. Synchronization mechanisms: semaphores, locks, wait/notify

## Introduction
The key components of the terminal will be represented as objects or threads and the activities that occurs will be translated into functions. Firstly, the 2 entrance guards will be represented as 2 individual threads. Similarly, the customers will be represented as threads so that they can run concurrently, making progress at the same time. This is suitable for customers as they carry out most of their activities in the terminal at the same time. The West-Entrance-Guard-Thread will share an object with the customer threads, which is the West-Entrance-Object. Similarly, the East-Entrance-Guard-Thread will share an East-Entrance-Object with customer threads, which represents the entrance of the terminal. In real life scenario, it simulates the interaction of entrance guard and customers through the entrance.

Next, for ticket acquiring process, there are 1 object as ticketing machine, 2 objects as the ticket counters and 2 threads as the ticket personnel. The 2 Ticket-Personnel-Threads will share the Ticket-Counters-Object with the customer threads. 

Furthermore, the waiting areas will be represented as 3 individual objects and the temperature scanner will be represented as an object. The ticket inspector will be represented as an object as it will be shared among the customer threads. Lastly, the buses will be represented as objects and the bus driver will be represented as thread. With that, the bus object will be shared among the customer threads and the bus driver thread. A detailed diagram is illustrated as shown in Figure 1 to display all the threads and objects that will be created for the concurrent Java program.

![Bus terminal simulation plan](https://github.com/jeerayuthleeseesuwan/java-concurrent-programming/blob/main/bus%20terminal%20simulation%20plan.png) 

