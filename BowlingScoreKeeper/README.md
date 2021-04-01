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
## Test Suite - Should Do
- [ ] I have carefully read the project specifications/requirements, as well as the setups in the test code (e.g., **@Before**, which runs before each **@Test**)
- [ ] I understand what are expected program behaviors (expected outputs) under certain circumstances (inputs), and my unit tests accurately reflect the intended testing scenarios
- [ ] I have written unit tests to test
  - [ ] Valid inputs
  - [ ] Boundary cases
  - [ ] Invalid inputs
  - [ ] Expected exceptions
## Test Suite - Chould Do
- [ ]
## Test Case - Should Do
- [ ] I have checked that every unit test is annotated with @Test.
- [ ] I have run my unit tests via “Run as JUnit Test”, and they either
  - [ ] pass consistently, or
  - [ ] reveal the presence of a bug in the source code
- [ ] I have checked that each unit test and it
  - [ ] has at least one assert statement (e.g., **assertTrue**, **assertFalse**, **assertEquals**) ([click for tutorials](https://www.baeldung.com/junit-assertions)) , or 
  - [ ] asserts an exception is thrown (e.g., **try{...; fail();} catch(Exception e){assertThat...;}**, **@Test(expected = exception.class)** in JUnit 4, **assertThrows** in JUnit 5) ([click for tutorials](https://www.baeldung.com/junit-assert-exception)). 
- [ ] I have tested only one method per unit test
## Test Case - Chould Do
- [ ] I have split up the unit tests that contains too many assert statements (e.g., split via **@Before** when there are more than five assertions)
- [ ] I have descriptively and explicitly
  - [ ] named my unit tests
  - [ ] commented my unit tests
