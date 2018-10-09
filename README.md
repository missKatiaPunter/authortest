# Documenting Tape
><small> **Note:** This is a **document authoring recruitment test** for 27 partners.</small>
## What is Tape?

**Tape** is a library for testing JavaScript code. It was written by **James Halliday**, aka [*substack*](https://substack.net/). Full code and the original documentation can be found [*here*](https://github.com/substack/tape).

Being a beginner friendly framework, Tape is great for learning to write **unit tests**. Unit tests are small, automated tests that compare the actual output from individual units with expected output. A unit is often, if not usually, a single function. In order to be testable a function should produce predictable results. Expected value **5**, for instance, can be used to test the following function:
```js
function addTwoAndThree() {
  return 2+3;
}
```
Tape is known as the ‘bare minimum’ testing framework. As such it is lightweight, with no configuration required and free from global variables such as `describe`. Tests produced with Tape are JavaScript files and can run in Node or in a browser.

Tape produces **TAP output**. **TAP** stands for **Test Anything Protocol**, it is documented [*here*](https://testanything.org/). It was originally designed to test Perl code in the late 1980s. A protocol is a standardised way of doing something, in case of TAP reporting the outcome of unit tests. A classic example of a protocol is meeting the Queen: call her ‘Ma’am’ (like in *"jam"*). TAP prescribes the following reporting from a test:

+ 1..***n*** reports the number of tests run with n being the number of tests
+ **ok 1** <message> - means that the frst test was successful
+ **not ok 2**  <message> - means that the second test failed

The screenshot below shows the TAP output produced by running two successful tests. The words ‘Test description’ are placeholders, here the test author should write concise and meaningful explanations of functionality being tested.

![tap-output](https://user-images.githubusercontent.com/18426161/46638963-61ea2f00-cb5b-11e8-9d5c-383f92c53b22.png)

Failing tests will produce exceptions, messages outlining why tests were not successful. If one previously experienced a less minimalist testing framework they might be left disappointed: standard TAP output has no color coding, no timings, no file or function names, no line numbers. On the brighter side, if one is used to deciphering TAP output for JavaScript test, they will be able to understand TAP producing tests of other programming languages.

Another limitation of Tape and TAP is a small number of built-in assertions. Built-in assertions are methods included in the testing library that allow to compare the expected outcome of a unit with its actual outcome.

### Boolean assertions included in Tape

```js
var test = require("tape");

test("Check that true is truthy", function (t) {
  t.ok(true, 'True is true');
  t.end();
});
```

## Setting up the environment

## Your first tests
