# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > Let, Const, Var

02. What is the definition of a function?

    > Seperate code that is designed to run a certain task, will not be ran unless called or invoked.

03. What are the `SOLID` principles?

    > Single Responsability principle, Open Closed principle, liskov substitution principle, Interface segregation principle, and Dependency Inversion Principle

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```
<!-- NOTE -->
    > fruit.splice('pineapple')

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```
<!-- NOTE -->
    >   you.friends.push(them)

06. Give an example of a JavaScript `Conditional`:

    > If, Else

07. What is the main difference between `parameters` and `arguments`?

    > Parameters are the names created in function definition and arguments are the values the definition receives.

08. Instead of writing everything to the console, what is a better way to debug your code?

    > Use chromes built in developer tools.

09. What is the difference between a `primitive` value and a `reference` value?

    > primitive values are values you can change or delete, while reference values you can not.

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > for (let i = -100; i < 101; i++) {
  const element = [i];
  console.log(i)
}
