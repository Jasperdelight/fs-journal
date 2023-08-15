# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | It's our little envelope containing all the information of that page, so a page that holds a collection of related classes and function and other things. For example you wouldn't have something to do with houses in a cars namespace. |

02. What is the difference between a `class` and an `interface`?

  > | A class is a schematic for creating objects while interface is the what that class does, classes can have many interfaces or "jobs" is one way of looking at it.|

03. What is the method that returns an instance of a class, yet it has no return type?

  > | A constructor would return an instance of a class but it itself has no type. |

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

  > | public, there are other access modifiers like private and internal |

06. In the Car example what is `string` an indication of?

  > | What the return type will be from the function |

07. In the Car example what is `abstract` preventing?

  > | It prevents malicious users from instantiating an instance of that class when they're not supposed to be. Its another way to keep data safe and "abstract" it away from users. |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | Information in a column is the types of data, so like a houses bedrooms, bathrooms ect. the row is the actual values of the columns. So like how many bedrooms and bathrooms that particular house would have as well as the contents of its Id |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > | CREATE TABLE characters (
    id INT PRIMARY KEY NOT NULL AUTO_INCREMENT,
    name VARCHAR(255) NOT NULL,
    age INT UNSIGNED DEFAULT 0,
    description VARCHAR(255) NOT NULL
  )default charset utf8 COMMENT ''; |

10. In SQL how can you query more than a single table? Provide an example.

  > | You can do so by using the JOIN operations to combine the data from multiple tables, so if i wanted to make a bundle deal on gregslist with cars and houses i would first target the tables i want to combine. Then from shows what data table i want to be the main one. Then INNER JOIN specifies what table i'm joining on my main one and ON signifies what keyword will be used to show the relationship between the two peices of data from the seperate tables.
   So 
  SELECT houses.Id , cars.Id
  FROM houses
  INNER JOIN cars ON houses.cars_Id = cars.cars_Id|
