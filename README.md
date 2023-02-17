EX1

![image](https://user-images.githubusercontent.com/122611575/219639528-95d45747-2916-4b33-9d86-6654d3dd3afd.png)

INSERT INTO terms VALUES (6, 'Net due 120 days', 120)

Inserted a new record 


EX2

![image](https://user-images.githubusercontent.com/122611575/219639746-876cddb0-4d41-40f1-9b89-81ce55ff6526.png)

UPDATE terms
SET terms_description = 'Net due 125 days',
terms_due_days   = 125
WHERE terms_id = 6

Updated the record from ex1


EX3

![image](https://user-images.githubusercontent.com/122611575/219640053-459a56b2-216a-4a82-b30a-f8461c39eedb.png)

DELETE FROM terms
WHERE terms_id = 6

Deleted the record from ex 1+2


EX4

![image](https://user-images.githubusercontent.com/122611575/219640170-219edd97-e21c-493e-8724-8d3bdee86725.png)


INSERT INTO invoices VALUES 
(AUTO_INCREMENT, 32, 'AX-014-027', '2018-08-01', 434.58, 0.00, 0.00, 2, '2018-08-31', NULL)

Inserted a new record into the invoices table with out a column list


EX5

![image](https://user-images.githubusercontent.com/122611575/219640332-56eb1ebc-16c2-4dd3-9f21-0bbec8aeb413.png)


INSERT INTO invoice_line_items VALUES
(115, 1, 160, 180.23, 'Hard drive'),
(115, 2, 527, 254.35, 'Exchange Server update')

Inserting two records at the same time


EX6

![image](https://user-images.githubusercontent.com/122611575/219640538-7d056eaa-9a4e-4cb0-93bb-b8a55cbd457c.png)


UPDATE invoices
SET credit_total = invoice_total * .1
UPDATE invoices
SET payment_total = payment_total + credit_total = invoice_total

Updating two columns at the same time


EX7

![image](https://user-images.githubusercontent.com/122611575/219640656-9d685ea5-3b9c-4c70-85ce-0eb8888cd37b.png)


UPDATE vendors
SET default_account_number = 403
WHERE vendor_id = 43

Updating a particular cell in a table


EX8

![image](https://user-images.githubusercontent.com/122611575/219640751-0b7114bd-9f7e-43aa-988d-1c34d34a9af1.png)


UPDATE invoices, vendors
SET terms_id = 2
WHERE default_terms_id = 2

Updating two tables at the same time

EX9

![image](https://user-images.githubusercontent.com/122611575/219640880-cb949266-3849-4651-acfc-d24ae71c8c89.png)

DELETE FROM invoice_line_items
WHERE invoice_id = 115;
DELETE FROM invoices
WHERE invoice_id = 115

Delete a record from two tables at the same time
