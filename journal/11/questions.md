# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | It allows the derived class to inherit almost all the properties and functions of a base class.|

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | Member inheritance works by the parent inheriting the child, a class does not inherit all members of the base class. for instance constructors and finalizers aren't inherited.|

3. How does ***accessibility*** affect inheritance?

  > | Accessibility affects inheritance by determining what is accessible from subclasses or other classes. So these would be the public and private that we declare when we make functions and respositories/controllers/services and many other things.|

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | The primary key is the unique identifier for each class while a foreign key is a reference to another classes primary key for establishing connections with other tables|

5. What is an ***alias***?

  > | An alias would be a temporary name assigned to a table or a column in a query result. Helps make queries more readable. |

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > | SELECT 
  p.*
  d.*
  FROM patients p
  LEFT JOIN patient_doctors patdoc ON p.id = patdoc.patientId
  JOIN doctors d ON patdoc.doctorId = d.id;
  
       |
