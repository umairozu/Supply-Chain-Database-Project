Project Description:
============
We are going to design a system to manage supply-chain of customer companies.
Some classes will already be provided with the desired methods. 
You need to implement all functionalities listed in Requirements section.
This may require you to implement methods given in the template code, write new classes, methods and all necessary code.
The codes will be tested with a private set of tests (different than the ones provided to you).

Requirements
============
1. We should be able to find, add and delete companies.
2. Each company will have 
  * name: its identifier
  * address: country, city, zip number and street info. If zip number is same, then the city must be the same.
  * phone number: Each company must have exactly one phone number, and two company cannot have the same phone number
  * e-mail: A company may have zero or more e-mail address
3. We should be able to find, add, delete and update products.
4. Each product will have an id, name, description and brand name
  *	Products are identified by their ids. 
  *	The system should not accept products with no name.
5. A company has a capacity to produce a product. If the ordered transaction amounts are more than the production capacity, the order should not be accepted.
6. The system accepts orders for products and send them to companies. Each order has an amount and order date information.
  * If the total active orders exceed the production capacity of company, it should automatically be rejected.
7. When the ordered amount of product is shipped by the company, the order is deleted from active orders, but the transaction information is not lost. The old transaction information should be stored in transaction_history for further analysis.
 * (Query1) The system shall track the list of product IDs ordered the most for each company.
 * (Query2) The system shall track the inactive companies (i.e., their name) for a given time period. E.g., the companies which does not have any order between given two dates.
8. The system shall implement the predetermined REST calls. Please see controller package for further information.
 * ALL REST CALLS MUST BE TRANSACTIONAL. PLEASE MAKE SURE THAT ACID PROPERTIES ARE SATISFIED!


Submission
==========
ER-diagram, relational model documentation are available under docs

NOTE
====
Intellij IDE, JAVA 14 and Maven are used 
