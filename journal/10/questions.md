# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | to organize code and to make it not confusing  |

02. What is the difference between a `class` and an `interface`?

  > | a class has both definitions and interface only has a definition |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | The method that returns an instance of a class is called a method |

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > | the method is accessible from outside the car class |

06. In the Car example what is `string` an indication of?

  > | its an indication of a returned string |

07. In the Car example what is `abstract` preventing?

  > | it is preventing the creation of an instance of car |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | column arranges data vertically and a row arranges from left to right  |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > | CREATE TABLE characters (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(50) NOT NULL,
    age TEXT,
    description VARCHAR(100) NOT NULL UNIQUE |

10. In SQL how can you query more than a single table? Provide an example.

  > | you can use subqueries ex: SELECT column1 FROM table1 WHERE EXISTS (SELECT column1 FROM table2 WHERE table1. column1 = table2)
