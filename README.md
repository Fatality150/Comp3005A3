# Comp3005A3

Author: Owen Hobbs
SN: 101197523

To run, download the IntelliJ ide and open the porject, then nevigate to main.java (/src/main/java/Main.java), and execute by pressing the green 'run' icon

IntelliJ website: (available free through the community edition)
https://www.jetbrains.com/idea/download/?section=windows

Database Creation Code

create table students
(
    student_id serial,
    first_name text not null,
    last_name text not null,
    email text not null unique,
    enrollment_date date,
    primary key (student_id)
);

in pgadmin4 create a databse with the name of A3, right click and select query tool, input the code provided above, and after the code below to create and populate a databse to be queried using the code found in this git.

Database Data Code

INSERT INTO students (first_name, last_name, email, enrollment_date) VALUES
('John', 'Doe', 'john.doe@example.com', '2023-09-01'),
('Jane', 'Smith', 'jane.smith@example.com', '2023-09-01'),
('Jim', 'Beam', 'jim.beam@example.com', '2023-09-02');

Video showing functionality:
https://youtu.be/iZCiwRzQ258
