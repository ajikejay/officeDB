CREATE TABLE employee (
    employee_id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    department_id INT NOT NULL,
    salary DECIMAL(10,2) NOT NULL
);

INSERT INTO employee (employee_id, name, department_id, salary)
VALUES (1, 'John Doe', 1, 50000),
       (2, 'Jane Doe', 2, 60000),
       (3, 'Bob Smith', 1, 70000),
       (4, 'Sally Smith', 2, 65000),
       (5, 'Helen Carl', 4, 85000),
       (6, 'Mary Wood', 3, 115000),
       (7, 'Elton Cross', 5, 117000);
       
      CREATE TABLE departments (
    department_id INTEGER PRIMARY KEY,
    name VARCHAR(255),
    manager VARCHAR(255)
);

INSERT INTO departments (department_id, name, manager) VALUES (1, 'Accounting', 'John Smith');
INSERT INTO departments (department_id, name, manager) VALUES (2, 'Marketing', 'Jane Doe');
INSERT INTO departments (department_id, name, manager) VALUES (3, 'IT', 'Tim Cook');
INSERT INTO departments (department_id, name, manager) VALUES (4, 'HR', 'Sarah Lee');
INSERT INTO departments (department_id, name, manager) VALUES (5, 'Sales', 'Mark Davis');


CREATE TABLE salaries (
    employee_id INT NOT NULL,
    amount NUMERIC NOT NULL,
    start_date DATE NOT NULL,
    end_date DATE
);

INSERT INTO salaries (employee_id, amount, start_date, end_date)
VALUES (1, 50000, '2022-01-01', '2022-12-31'),
       (2, 20000, '2022-01-01', NULL),
       (3, 70000, '2022-01-01', '2022-12-31'),
       (4, 65000, '2022-01-01', '2022-12-31'),
       (5, 85000, '2022-01-01', '2022-12-31'),
       (6, 115000, '2022-01-01', '2022-12-31'),
       (7, 117000, '2022-01-01', '2022-12-31');

