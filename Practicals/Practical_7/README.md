
---

# Sequence Diagram: Car Rental System

This sequence diagram illustrates the interaction between various components involved in processing a car rental request.

![alt text](image.png)

---

##  Actors & Components

- **Desk Officer**: Staff member responsible for handling customer requests.
- **Rent Car Screen**: User interface used to input and manage rental operations.
- **Validation Services**: Component responsible for validating user input like contact number and CID (Citizen ID).
- **Car Inventory**: Manages available cars and their rental status.
- **Customer Database**: Stores customer details.
- **Rental Database**: Stores rental transaction records.
- **Billing System**: Sends rental information to the customer.

---

##  Flow Description

1. **Input Request**  
   The *Desk Officer* enters the customer’s details and car requirements into the system via the **Rent Car Screen**.

2. **Validation**  
   The system sends the entered **Contact Number** and **CID** to **Validation Services** for verification.

3. **Validation Response**  
   The **Validation Services** responds with either a **valid** or **invalid** status.

4. **Validation Failure Handling**  
   If the data is invalid, an error message is displayed back to the **Desk Officer**.

5. **Car Availability Request**  
   If valid, the **Rent Car Screen** requests available cars from the **Car Inventory**.

6. **Availability Response**  
   The **Car Inventory** responds with car details that match the requirements.

7. **Update Car Status**  
   The chosen car’s status is updated to `"rented out"` in the **Car Inventory**.

8. **Customer Record Save**  
   The customer’s information is saved in the **Customer Database**.

9. **Rental Record Creation**  
   A new rental record is created and saved in the **Rental Database**.

10. **Send Confirmation**  
    The **Billing System** sends the rental record/confirmation to the customer.

11. **Success Message**  
    A success message is displayed to the **Desk Officer**, confirming the rental is complete.

---

##  Notes

- This process ensures input validation before reserving any vehicle.
- The **Car Inventory** is updated in real time to prevent double-booking.
- The system maintains separation of concerns via dedicated services (e.g., Validation, Rental DB, Billing).
- The diagram follows a synchronous interaction pattern.
