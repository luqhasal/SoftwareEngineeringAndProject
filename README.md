Lunar Rover Mapping Robot.

Video demonstration link: https://youtu.be/M5fhArJOS-I

Sample project from Software Engineering and Project module.

#### Lunar Rover Mapping Robot

The Lunar Rover Mapping Robot project is a challenge initiated by the Google’s Lunar XPRIZE. Having the use of the low-cost method of robotic space, it aims to locate and gather the details of the Apollo 17 and its remnants which was landed on the Moon in December 1972. 

Our focus in this project is to create a prototype Lunar Rover using the Lego Mindstorm EV3 kit and integrate it with a JAVA system. This prototype shall simulate in an real-time environment of a small area of the Moon. The surveying area shall be a bounding box of 500 meters. The Lunar Rover shall have the capability to determine the remnants of the Apollo 17 within the stipulated time, and distinguish between mapped and unmapped regions. Some of the important features such as safety policy and operation controls shall be implemented into the system.

#### Project Structure

    ├───build             # Compiled files
    │   └───rover
    │   └───system
    ├───docs              # Documentation files, with sub-directories for different documentations
    │   ├───cr
    │   ├───meetings
    │   │   ├───agenda
    │   │   └───minutes
    │   ├───sdd
    │   ├───spmp
    │   └───srs
    │   └───test-report
    │   └───user-manual
    ├───src               # Source files, with sub-directories for modules
    │   └───rover
    │   └───system
    │   └───lib
    ├───test              # Automated tests, with sub-directories for modules
    ├───tools             # Tools and utilities, with sub-directories for different tools
    │   └───eclipse
    ├───build.xml         # Ant build file
    ├───README.md         # Information on Git repository main page
    └───LICENSE.md        # MIT license

#### Coding Convention

For Coding Convention, the "[Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)" shall be adopted partially.

This allows for good readability which is important as everyone shall be part of the development team.

In general, these should be followed.

#### Source Files
- Encoded in **UTF-8**
- Case-sensitive file names of the top-level class with .java extension
- Special escape with backslash. (\b, \t, \n, \f, \r, \\", \\' and \\\\)
- Do not use octal (\012) or unicode escape (\u000a)
- Use whitespaces only. Do not use tab for indentation

#### Source Code Structure
- Do not use wildcard for Import Statements (e.g. do not use import java.lang.Math.*)

#### Formatting
- 2-spaces indentation
- Use braces for (if, else, for, do and while) statements, even when containing single line of code
- Linebreaks & Braces:
    - No line break before the opening brace
    - Line break after the opening brace
    - Line break before the closing brace
    - Line break after the closing brace, only if that brace terminates a statement or terminates the body of a method, constructor, or named class. For example, there is no line break after the brace if it is followed by else or a comma
    - Example:
    
```
    return new MyClass() {
      @Override public void method() {
        if (condition()) {
          try {
            something();
          } catch (ProblemException e) {
            recover();
          }
        } else if (otherCondition()) {
          somethingElse();
        } else {
          lastThing();
        }
      }
    };
```

#### Naming

- Class names:
    - UpperCamelCase
    - Usually in nouns
- Test Class names:
    - Class name + "Test"
    - Example: UpperCamelCaseTest
- Method names:
    - lowerCamelCase
    - Usually in verbs
- Constant names:
    - CONSTANT_CASE
    - All uppercase and words separated by underscore
- Non-constant field names:
    - lowerCamelCase
- Parameter names:
    - lowerCamelCase
- Local variable names:
    - lowerCamelCase
