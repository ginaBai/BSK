Bowling Scorekeeper
===
The objective is to TEST an application that can calculate the score of a single bowling game.
- There is no graphical user interface.  
- You work ONLY with JUnit test cases in this project.
- You have ONE HOUR to work on this project.
- You are free to consult/use any online resources, including documentations, tutorials, Q&A sites, and any Eclipse built-in tools or plug-ins.
 

**Project Template**  
You are provided with a completed project that contains three classes: `Frame`, `BowlingGame` and `BowlingException`, each contains some fields and methods. DO NOT CHANGE the names and functionalities of the existing fields and methods.

You are expected to create JUnit test cases to verify the behavior of this implementation as thorough as possible based on the following description of a bowling score keeper. Your program should throw `BowlingException` in all error situations. 

**Bowling Score Keeper Task Description**  
The game consists of 10 frames as shown below. In each frame the player has two opportunities to knock down 10 pins. The score for the frame is the total number of pins knocked down, plus bonuses for strikes and spares.

![ExampleImage](https://github.com/ginaBai/BSK/blob/master/BowlingScoreKeeper/BowlingScoreKeeperExample.png)

A spare is when the player knocks down all 10 pins in two throws. The bonus for that frame is the number of pins knocked down by the next throw. So in frame 3 of the example game below, the score is 10 (the total number knocked down) plus a bonus of 5 (the number of pins knocked down on the next throw).

A strike is when the player knocks down all 10 pins on his first try. The bonus for that frame is the value of the next two throws. 

In the tenth frame, a player who rolls a spare or strike is allowed to have bonus throws to complete the frame. However, no more than three balls can be rolled in tenth frame.

**Examples**  
[Click for Detailed Rules and Examples of Scoring a Game of Bowling](https://slocums.homestead.com/gamescore.html)

[Online Bowling Game Score Calculator](https://bowlinggenius.com)


# Checklist

For each test case, use the following guidelines:
## Each Test Case - Should Do
- [ ] The unit test is annotated with **@Test**.
- [ ] The unit test is executable (e.g., via “Run as JUnit Test”)
- [ ] The unit test has at least one assert statement (e.g., **assertTrue**, **assertFalse**, **assertEquals**) ([click for tutorials](https://www.baeldung.com/junit-assertions)) , or it asserts an exception is thrown (e.g., **try{...; fail();} catch(Exception e){assertThat...;}**, **@Test(expected = exception.class)** in JUnit 4, **assertThrows** in JUnit 5) ([click for tutorials](https://www.baeldung.com/junit-assert-exception)). 
- [ ] The unit test evaluates/tests only one method
## Each Test Case - Could Do
- [ ] If there are too many assert statements, split it up (e.g., using **@Before** when there are more than five assertions)
- [ ] The unit test is descriptively named and commented

Considering the entire test suite (all your test cases together), use the following guidelines: 
## Test Suite - Should Do
- [ ] Ensure each requirement is tested
- [ ] Ensure the setup and teardown code with the test suite is used appropriately (e.g., **@Before**, which runs before each **@Test**)
- [ ] For each bug in the code, ensure there is a fault-revealing test (i.e., one that fails)
- [ ] For each requirement, ensure unit tests exist for:
  - [ ] Valid inputs
  - [ ] Boundary cases
  - [ ] Invalid inputs
  - [ ] Expected exceptions
## Test Suite - Could Do
- [ ] Measure code coverage using an appropriate tool, such as EclEmma ([installation](https://www.eclemma.org/installation.html), [tutorial](https://www.eclipse.org/community/eclipse_newsletter/2015/august/article1.php)). Inspect uncovered code and write tests as appropriate.
