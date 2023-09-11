# SQL_ACID_TRANSACTION_AND_STORED_PROCEDURE_IMPLEMENTATION
About project: In an ACID transaction, if any of these actions fail (for example, if your payment doesn't go through), then the entire transaction fails and none of the changes are made. This ensures that the data in the database remains consistent.
Benefits: ACID transaction is a way to ensure that a group of actions in a database either all happen successfully or none of them happen at all.

Project case study: 
Let's say you're buying a pair of boots online. When you make the purchase, several things need to happen: the boots need to be added to your cart, your payment needs to be processed, your account needs to be debited the correct amount, the store's account needs to be credited, and the inventory of boots needs to be reduced by one.
- Created a stored procedure routine named TRANSACTION_ROSE which will include TCL commands like COMMIT and ROLLBACK, developed the routine based on the given scenario to execute a transaction. Scenario: Let’s buy Rose a pair of Boots from ShoeShop. So we have to update the Rose balance as well as the ShoeShop balance in the BankAccounts table. Then we also have to update Boots stock in the ShoeShop table. After Boots, let’s also attempt to buy Rose a pair of Trainers.
- Created a stored procedure TRANSACTION_JAMES to execute a transaction based on the following scenario: First buy James 4 pairs of Trainers from ShoeShop. Update his balance as well as the balance of ShoeShop. Also, update the stock of Trainers at ShoeShop. Then attempt to buy James a pair of Brogues from ShoeShop. If any of the UPDATE statements fail, the whole transaction fails the transaction rolls back and commit the transaction only if the whole transaction is successful.
