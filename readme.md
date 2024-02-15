**Report on Database Modeling for Mechanical Workshop**

**Introduction:**
This report presents the database modeling for a mechanical workshop, developed with the aim of controlling and managing the execution of service orders. The modeling was carried out based on a narrative that describes the typical operations of a mechanical workshop, from the reception of the vehicle to the completion of the services provided.

![photo](/mechanicalworkshopdb.png)

**Methods:**
The database modeling was performed using the SQL language, specifically the MySQL database management system. The process involved identifying the main entities involved in the context of the mechanical workshop, such as customers, vehicles, mechanics, and service orders. Then, the attributes of each entity and the relationships between them were defined, ensuring data integrity and system efficiency.

**Results:**
The conceptual schema of the database includes the following main entities:

1. **Customer:** Stores information about workshop customers, such as name, phone, and address.
2. **Vehicle:** Registers customers' vehicles, including information such as license plate, model, and year.
3. **Mechanic:** Contains data on workshop mechanics, such as name, address, and specialty.
4. **Service Order (OS):** Responsible for recording service orders issued by customers, with information such as issue date, total value, status, and completion date.
5. **Service:** Describes the services offered by the workshop, including a description and value.
6. **Part:** Registers the parts used in the services provided, with name and value.

Additionally, the following relationships were established:

- A customer can have multiple vehicles, but a vehicle belongs to only one customer.
- A service order is associated with a single vehicle.
- A mechanic can be assigned to several service orders, but a service order has only one responsible mechanic.
- A service order can contain multiple services and parts.

**Conclusion:**
The database modeling for the mechanical workshop was designed to meet the needs of controlling and managing service orders in an efficient and organized manner. The proposed structure allows for detailed registration of relevant information, such as customers, vehicles, services provided, and mechanics involved, ensuring comprehensive management of the vehicle maintenance and repair process.

**Case Study:**
Suppose a customer, John Smith, brings his vehicle to the workshop for repairs. After evaluation by the mechanics' team, a service order is issued with an issue date on 02/10/2024 and an initial total value of $500. The service order is assigned to mechanic Carlos Santos. During the execution of the services, three different types of services are performed, and two specific parts are used. After completion of the work, the service order is marked as "Completed" on 02/15/2024. All this data is properly recorded in the database, allowing for effective monitoring and management of John Smith's vehicle repair process at the mechanical workshop.
