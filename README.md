# CodePerfect
Learning to write quality code together

- The place where i collect and list good coding principles and supply collections of good resources to learn that
- Covers universally accepted principles independent of a language though samples from C++, Python, and Java will be here for practical reasons


Code is more often read than written. I definitely agree with that as we all first read a lot of our own code, and then as we mature on software engineering - we inevitably read a lot of the others' code. So, why not make this reading process a pleasant activity for everyone?

**Good code code should speak for itself** bringing in this concept of self-documenting code where much of the explanation what the code does comes from the actual proper namings: constants, variables, classes, methods & functions, modules & packages. Definitely checkout this [naming cheatsheet](https://github.com/kettanaito/naming-cheatsheet) on the universal rules and good practices.

[Here](https://realpython.com/python-code-quality/) you can read about good Python code quality with some of the popular tools for that. 

### Standards: a way for beginners
I share the opinion that for beginners it is best to stick to the widely accepted standards, e.g. Python's PEP8 or Java's standards and common practices.
- [Java Code Conventions (1999)](https://www.oracle.com/technetwork/java/codeconventions-150003.pdf)
- [Python Style Guide (PEP-8) Explained](https://realpython.com/python-pep8/)
- [C++ Core Guidelines](https://github.com/isocpp/CppCoreGuidelines)
### Your project standards
Many teams have a bit of their own flavor and understanding what makes a good code for their particular project. Companies may even introduce internal well-written guidelines and practices. Such practices may include individual project-induced practices and code samples, such as those developed over time and started by the core team, for example.

As an example, in Python's Django framework some teams introduce the service layer that can be written in various ways. Other projects may treat this as extra-complexity and implement their business logic in the view layer.

### Framework-imposed styles
Frameworks impose their own code-writing style; what may be excessive in naming, for example, may in fact be an accepted practice within a particular framework itself.

## Fundamental Principles
Targeting reusability, team cooperation, and maintenance with scalability
- Don't Repeat Yourself - the DRY principle - main goal to reduce duplication within a system (amongst its various components)
- SOLID principles

Quick summary of Robert Martin's Clean Code - [cheat sheet](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29)<br>
or the book itself (but you can find a version online) - [Amazon](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882)

### Orthogonality
We all remember from high school that two vectors are called orthogonal to each other if they meet at a 90-degree angle. It's just a fancy word for perpendicular. You make a change in one direction, and the other part isn't affected by that change.

Simple test for orthogonality: *If my requirements experience subtle changes, how many layers (modules/functions) in my code will be affected by that change?*<br>
The fewer the better, with a theoretico-magical of 1.

## Commenting & documenting your code
As the authors of *The Pragmatic Programmer* have correctly put it - *"...bad code required lots of comments."*

Even though good code should speak for itself, there are inevitable places in code where comments and documentation take over. This becomes essential in public projects and within a team, once you go out the code-for-yourself mode. But even in this mode, reading your code after a few months you want to make sure you won't be asking yourself a question like: *Why the hell did I write that?* I find comments applicable where it isn't completely obvious why I wrote a line of code such as hacks in my algorithms solvers.

For example, in my series of solving algorithmic problems I find this helpful in solving the [car fueling problem](https://github.com/dron-dronych/python-algorithms/blob/master/greedy/car_fueling.py):

```python
stops = [arg for arg in args]
stops.append(distance)  # last point on the route
```
or
```c++
int stops [n_stops + 2]; // add origin & destination points to stops
```

As the project goes, so does your knowledge that might be already spread across different modules. This includes comments whose amount grows as well introducing more **space and time** for maintenance. Unnecessary comments in one place (especially with modules duplicated across the project) will have to be undoubtedly taken care of with new requirements or bug fixes.

## Collaborating

Gitlab offers a good [guide](https://learn.gitlab.com/c/version-control-best-practice?x=-RIZtH) on version control best practices.

The have also developed a well written [guide](https://learn.gitlab.com/smb-vcc-1/branching-strategies) on branching strategies.

## Architectural Patterns
One interesting read on objections to the service layer from the Service-Oriented Architecture in Django applications: [Against Services in Django](https://www.b-list.org/weblog/2020/mar/16/no-service/)

[High-level look at 5 architectural patterns](https://dzone.com/articles/5-major-software-architecture-patterns)

[Application Architecture Patterns Guide](https://docs.microsoft.com/en-us/previous-versions/msp-n-p/dn600223(v=pandp.10)) by Microsoft on 24 application architecture patterns with in-depth look at each and use cases

DISCLAIMER

*This guide is being developed as part of the learning process and all your comments and suggestions are highly welcomed!*


