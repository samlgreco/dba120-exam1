EX1

INSERT INTO terms VALUES (6, 'Net due 120 days', 120)

inserted a new record 


EX2

UPDATE terms
SET terms_description = 'Net due 125 days'
terms_due_days   = 125
WHERE terms_id = 6

Updated the row from ex1


EX3

DELETE FROM terms
WHERE terms_id = 6

Deleted the row from ex 1+2


EX4
