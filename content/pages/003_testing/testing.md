Title: Testing
Lang: en
Category: testing
Slug: testing
Summary: How to test your code
Status: published

There are many ways to test your code. The good news is that you have probably already done it many times – every time you make a change to your script/application then run it, that is testing. This, in particular, is called manual testing.

Another form of testing is known as automated testing, and this relies on another script to test your code (usually done with a testing framework). You can find recommendations to some testing frameworks below under "Language-Specific Conventions" in the "Package Recommendations" sections.

There are two kinds of automated testing: unit tests and integrated tests. Unlike integrated tests, which tests multiple functionalities together, a unit test will (ideally) focus on one functionality only, and prove it correct. Unit tests are useful for instances such as when you make a change to the code and the script/application breaks; your testing suite should then help pinpoint where the bug could be.

*TODO: insert animated gif here*
<figure>
<img></img>
<figcaption>Integrated test: will the door stay closed? Unit test: does the lock slider move to the left?  As we can see, the lock slider does slide over as expected, so we know that it isn't the locking component that is the issue - what could be allowing the door to open?!</figcaption>
</figure>

When writing a unit test, it is best practice (SHOULD?) to name it according to the component it is testing (prefixed by test). It will also be useful to add additional tests that will focus on different behaviors, expected errors, or edge cases, with the name reflecting that check, e.g

| Component | Test | Description |
|-|-|-|
| `def divide(m, n)` | `def test_divide()` | Does calling the function divide the two params? |
|| `def test_divide_by_zero_err()` | Does dividing by zero result in an error? |

Another good rule-of-thumb is to try and avoid test interdependence if you can; meaning, every test should have its own setup and tear-down. *TODO: define setup and tear-down.* You should write tests with the assumption that the state will not be maintained between each test. Otherwise, you may get hit with test failures that you did not encounter before (since test runners like to work in whatever order they please).

Finally, every new feature added to your script/application should include one or more unit tests – try to not save writing all tests for the end (it'll get crazy!). That is, every push to the repository that includes a new feature should also come with at least one unit test.

And remember: unit tests SHOULD focus on asserting the results and outcomes of the functionality, not the steps on how to get there. If you ever find that setting up a unit test for a particular functionality becomes cumbersome, e.g. it is getting complexingly difficult to set up a method in order to test it, you may want to revisit the design of your code.  In fact, this is one of the greatest things about unit tests – they provide excellent feedback on your approach and design.

