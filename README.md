https://memory-1utf.onrender.com/  (this is the link of deployment)


THIS IS MEMORY DOCUMENTATION
===========================
MEMORY DOCUMENTATION
UWERA Brigitte 23814

Project Overview:
This project revolves around the efficient acquisition of burial land, aiming to eliminate the stress associated with delayed or subpar burial services. Customers can request land from sellers based on their preferences, and the seller manages the customer information in a database. Once the customer completes the payment, they receive a confirmation message, and the available land count decreases accordingly. The primary goal is to streamline the land acquisition process, reducing waiting times and minimizing customer dissatisfaction.

Models:
1. Payment Model (Payment.java):
Attributes:
id: Payment ID
paymentCode: Unique payment code
tombId: Associated tomb for the payment
status: Payment status
paymentDate: Date of payment
customerId: Associated customer for the payment
listOfOtherServices: List of other services associated with the payment
2. Decease Model (Decease.java):
Attributes:
id: Decease ID
name: Name of the deceased
gender: Gender of the deceased
dob: Date of birth of the deceased
deceaseDate: Date of death
tombId: Associated tomb for the deceased
3. Customer Model (Customer.java):
Attributes:
id: Customer ID
email: Customer's email (unique)
names: Customer's name
password: Customer's password (hashed)
phoneNumber: Customer's phone number
role: Customer's role (USER/ADMIN)
listOfPayments: List of payments associated with the customer
Controller:
Payment Controller (PaymentController.java):
Endpoints:
POST /addPayment: Add a payment
POST /deletePayment: Delete a payment
Customer Controller (CustomerController.java):
Endpoints:
GET /customerInfo: Get information about deceases, tombs, and payments for a customer
POST /addPayment: Add a payment for a customer
POST /deletePayment: Delete a payment for a customer
POST /updatePayment: Update payment information for a customer
Implementation:
This project utilizes Spring Boot and Java for the backend, while the frontend is developed using HTML, CSS, and JavaScript.
 

Conclusion:
The project focuses on enhancing the burial land acquisition process, providing a seamless experience for customers. Through effective communication and streamlined procedures, the project aims to reduce waiting times and improve overall satisfaction.
Thank you!
