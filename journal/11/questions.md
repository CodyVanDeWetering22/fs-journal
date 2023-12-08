# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | You can make a Account and Profile class and inherit properties on other classes like id |

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | Yes all of the classes you have just extends off of the original class |

3. How does ***accessibility*** affect inheritance?

  > | if the class is private class it effects what some users see/get |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | primary key is used for the primary id in a class and a foreign key is using a different data on a different table like using creator |

5. What is an ***alias***?

  > | where the same thing can be accessed using different names  |

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
  doc*,
  pat*
  FROM patients
  JOIN patients pat ON pat.id = doc.id|
