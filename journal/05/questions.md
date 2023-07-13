# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > | Create, Read, Update, Delete |

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > | Create = Post, Read = Get, Update = Put, Delete = delete |

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > | ORM stands for Object-Relational Mapping. The schema part we use in mongoDB i believe would be considered an ORM when we interact with mongoDB. When we make a new schema we're making a new class thats oriented towards that one object type. Then we are using mongoDB's version of the CRUD methods on the schema of the object we want to change. |

04. Which two `HTTP` request types include a body?

  > | Post and Put |

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > | synchronous, async |

06. What are the three types of data relationships? Provide an example of each.

  > | one:one For example a person and their license. Each belongs to only the other. one : many is like book and its pages. one book but many pages. many to many is like authors and books, many authors make many books and books can have many authors |

07. What is middleware?

  > | functions that have access to the req, res objects and the next function when we call an api. How we are able to access things like req.body  |

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > | req, res |

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > | {baseURL}?tag=winter |

10. What is a ***virtual property***?

  > | A property we take from one model object then copy it onto a different one, or even compute new property altogether by using two properties from a different model object and merging them together.  |
