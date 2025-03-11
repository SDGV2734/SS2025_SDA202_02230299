# Architecture Charactersitic Worksheet for Road worrior 

![Alt text](<Screenshot 2568-03-10 at 11.14.52 PM.png>)

### 1. Driving Characteristic: Scalability 
(A function of system capacity and growth over time; as the number of users or requests increase in the system, responsiveness, performance, and error rates remain constant )

**Reason**

With reference to the requirment stating that the system will serve upto 10,000 + registered users worlwide and work internationally, the system must be able to scale efficiently meaning that, as the number of users or requests increase in the system, the system should not be latency. As users interact with the system, make frequent requests to third-party services (airlines, hotels, car rentals), and access their dashboards simultaneously and continously, the system should handle increasing loads easily.

**Use Case:**

When a major travel season occurs (e.g., holidays, business summits), the system should be capable of handling a increase in user activity without degradation in performance of the system. This means to ensure a smooth user experience. 

### 2. Driving Characteristic: Data Consistency
(The data across the system is in sync and consistent across databases and tables)

**Reason**

As the system will have to interface with multiple third-party services, it must ensure that the data about reservation remains  accurtate and sync throughtout the different sources. If a user's reservation changes (examle: flight reschedules, hotel booking modifications), these updates should be immediately reflected and get sync in their dashboard.

**Use Case**

If a traveler books a flight and a hotel under the same trip. And if the flight schedule changes, the system should immediately reflect this update, ensuring that the hotel reservation can be modified accordingly if needed. 

### 3. Driving Characteristic: Interoperability
(The ability of the system to interface and interact with other systems to complete a business request)

**Reason**

The system should seamlessly integrate with airlines, hotel, car rental services, and social media platforms. Since these third-party systems might use different data formats, authentication mechanisms, and APIs compared to our system so the system should be build in a flexible way to enable a smooth data exchange. 

**Use Case:**

A user might connect their frequent airline and hotel membership accounts to the system. The system must interact with various third-party APIs, fetch reservation details, and make the data format compatible to our system to display it on the dashboard.

