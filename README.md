# SQL-Constraints
DROP TABLE IF EXISTS test;

CREATE TABLE test (
id int,
a varchar(255),
b varchar(255),
Index(a),
Index(a,b))

INSERT INTO Test VALUES(1, 'one', 'two');
INSERT INTO Test VALUES(2, 'three', 'four');
INSERT INTO Test VALUES(3, 'five', 'six');

INSERT INTO test (
id int,
a varchar(255),
b varchar(255),
Index ab(a,b),
Index(a),
Index(b));

SHOW Indexes from Test;
DROP index ab on test;
