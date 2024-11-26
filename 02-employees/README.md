```SQL
CREATE TABLE IF NOT EXISTS Employee (
	employee_id SERIAL PRIMARY KEY,
	name VARCHAR(120) NOT NULL,
	department VARCHAR(150) NOT NULL,
	boss_id INTEGER REFERENCES Employee(employee_id)
);
```
