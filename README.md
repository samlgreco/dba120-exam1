EX1

INSERT INTO terms VALUES (6, 'Net due 120 days', 120)

Inserted a new record 


EX2

UPDATE terms
SET terms_description = 'Net due 125 days',
terms_due_days   = 125
WHERE terms_id = 6

Updated the record from ex1


EX3

DELETE FROM terms
WHERE terms_id = 6

Deleted the record from ex 1+2


EX4

INSERT INTO invoices VALUES 
(AUTO_INCREMENT, 32, 'AX-014-027', '2018-08-01', 434.58, 0.00, 0.00, 2, '2018-08-31', NULL)

Inserted a new record into the invoices table with out a column list


EX5

INSERT INTO invoice_line_items VALUES
(115, 1, 160, 180.23, 'Hard drive'),
(115, 2, 527, 254.35, 'Exchange Server update')

Inserting two records at the same time


EX6

UPDATE invoices
SET credit_total = invoice_total * .1
UPDATE invoices
SET payment_total = payment_total + credit_total = invoice_total

Updating two columns


EX7

