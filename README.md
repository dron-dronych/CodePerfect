# CodePerfect
Learning to write quality code together

- The place where i collect and list good coding principles and supply collections of good resources to learn that
- Covers universally accepted principles independent of a language though samples from C++, Python, and Java will be here for practical reasons


Code is more often read than written. I definitely agree with that as we all first read a lot of our own code, and then as we mature on software engineering - we inevitbaly read a lot of the others' code. So, why not make this reading process a pleasant activity for everyone?

**Good code code should speak for itself** bringing in this concept of self-documenting code where much of the explanation what the code does comes from the actual proper namings: constants, variables, classes, methods & functions, modules & packages.

### Standards: a way for beginners
I share the opinion that for beginners it is best to stick to the widely accepted standards, e.g. Python's PEP8 or Java's standards and common practices.
- [Java Code Conventions (1999)](https://www.oracle.com/technetwork/java/codeconventions-150003.pdf)
- [Python Style Guide (PEP-8) Explained](https://realpython.com/python-pep8/)
- [C++ Core Guidelines](https://github.com/isocpp/CppCoreGuidelines)
### Your project standards
Many teams have a bit of their own flavor and understanding what makes a good code for their particular project.
### Framework-imposed styles
Frameworks impose their own code-writing style; what may be excessive in naming, for example, may in fact be an accepted practice within a particular framework itself.

## Fundamental Principles
Targeting reusability, team cooperation, and maintenance with scalability
- Don't Repeat Yourself - the DRY principle
- SOLID principles

Quick summary of Robert Martin's Clean Code - [cheat sheet](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29)

## Commenting & documenting your code
Even though good code should speak for itself, there are inevitable places in code where comments and documentation take over. This becomes essential in public projects and within a team, once you go out the code-for-yourself mode. But even in this mode, reading your code after a few months you want to make sure you won't be asking yourself a question like: *Why the hell did I write that?* I find comments applicable where it isn't completely obvious why I wrote a line of code such as hacks in my algorithms solvers.

For example, in my series of solving algorithmic problems I find this helpful in solving the [car fueling problem](https://github.com/dron-dronych/python-algorithms/blob/master/greedy/car_fueling.py):

```python
stops = [arg for arg in args]
stops.append(distance)  # last point on the route
```

DISCLAIMER

*This guide is being developed as part of the learning process and all your comments and suggestions are highly welcomed!*


