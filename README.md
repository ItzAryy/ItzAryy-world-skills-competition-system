
# World Skills Competition System

A Java console application designed to manage a simulated skills competition using Object-Oriented Programming principles.

This project was originally developed as part of my Object-Oriented Programming coursework at Edinburgh College. The system manages competition information including colleges, teams, students, coaches, judges, projects and scores before calculating the final team rankings.

## Features

* Creates and manages a competition
* Stores college and team information
* Assigns students to teams
* Assigns coaches to teams
* Stores student projects
* Allows judges to award scores and feedback
* Calculates average project scores
* Calculates total team scores
* Automatically generates final team rankings
* Validates scores to ensure they remain between 0 and 100
* Displays competition information through a console report

## Object-Oriented Programming

The project was designed to demonstrate several Object-Oriented Programming concepts.

### Encapsulation

Class data is stored using private fields and accessed through methods where required.

### Inheritance

The system uses inheritance to share common behaviour between different types of people.

`Person` acts as a base class, with `Student` and `Coach` inheriting from it. `Judge` then inherits from `Coach`.

```text
Person
├── Student
└── Coach
    └── Judge
```

### Polymorphism

The `Judge` class overrides the `provideSupport()` method inherited from `Coach`, allowing different behaviour depending on the object type.

### Method Overloading

The `Project` class contains overloaded versions of the `calculateAverageScore()` method.

### Exception Handling

A custom `InvalidPoints` exception prevents judges from awarding scores below 0 or above 100.

## Main Classes

* `Main` - Creates the competition and connects the different objects
* `Competition` - Manages teams, judges and final rankings
* `College` - Stores college information and associated teams
* `Person` - Base class containing shared personal information
* `Student` - Stores student information and submitted projects
* `Coach` - Manages assigned teams
* `Judge` - Awards scores and provides feedback
* `Team` - Stores students and calculates the team's total score
* `Project` - Stores project information and calculates average scores
* `Score` - Stores marks and judge feedback
* `InvalidPoints` - Custom exception used for score validation

## Technologies Used

* Java
* Object-Oriented Programming
* Java ArrayList
* Java Comparator
* Exception Handling

## How It Works

The application creates a competition containing colleges, teams, students, coaches, judges and projects.

Students are assigned to teams and projects, while judges award scores and provide feedback for each project.

Project scores are used to calculate team totals. The teams are then sorted by their total score to produce the final competition rankings.

## Project Structure

```text
src/
├── Coach.java
├── College.java
├── Competition.java
├── InvalidPoints.java
├── Judge.java
├── Main.java
├── Person.java
├── Project.java
├── Score.java
├── Student.java
└── Team.java
```

## What I Learned

This project helped me develop my understanding of:

* Object-Oriented Programming
* Encapsulation
* Inheritance
* Polymorphism
* Method overriding
* Method overloading
* Java ArrayLists
* Relationships between classes
* Custom exceptions
* Exception handling
* Sorting objects using Comparator
* Breaking larger programs into multiple classes

## Future Improvements

* Add a graphical or web-based user interface
* Store competition data in an external database
* Allow competition data to be entered dynamically
* Support a larger number of teams and competitions
* Improve input validation and exception handling
* Add automated testing

## Screenshots

Screenshots of the application output will be added here.
