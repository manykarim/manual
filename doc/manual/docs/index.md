# Robot Framework Manual

## What is Robot Framework?  :simple-robotframework:

Robot Framework® is a generic open source automation framework for acceptance testing,
behavior-driven development (BDD) and robotic process automation (RPA). It has simple
[plain text syntax][syntax], and it can be [extended][extending-robot-framework]
easily with generic and custom [libraries][].

Robot Framework is operating system and application independent. It is implemented
using Python which is also the primary language to extend it. The framework has
a rich ecosystem around it consisting of various generic libraries and tools that
are developed as separate projects. For more information about Robot Framework and
the ecosystem, see https://robotframework.org.

## What is in this manual?  :blue_book:

Robot Framework Manual contains indepth information about all Robot Framework features
such as data syntax, how to execute tests and how to extend the framework.

The manual concentrates only to Robot Framework core and is rather technical.
If you are looking for more practical information related to getting started with
Robot Framework or using it in a certain domain such as web automation, see
the excellent [Robot Framework Guides](https://docs.robotframework.org/docs) project.

## Examples

These examples were added for testing syntax highlighting and can be removed.
Having some examples on the front page could be a good idea, though.

```robotframework
*** Settings ***
Documentation        Is this an interesting example?
Library              Example.py

*** Test Cases ***
Example
    [Documentation]    No, this this isn't.
    Greeting    Robot

*** Keyword ***
Greeting
    [Arguments]    ${name}
    IF    $name == "Robot"
        Log    Hello, good sir!
    ELSE
        Log    Hello, ${name}!
    END
```

```python
def greeting(name):
    if name == "Robot":
        print("Hello, good sir!")
    else:
        print(f"Hello, {name}!")
```
