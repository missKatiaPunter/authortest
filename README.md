# Documenting Tape
><small> **Disclosure:** This is a **document authoring recruitment test** for 27 partners.</small>
## What is Tape?

**Tape** is a library for testing JavaScript code. It was written by **James Halliday**, aka [*substack*](https://substack.net/). Full code and the original documentation can be found [*here*](https://github.com/substack/tape).

Being a beginner friendly framework, Tape is great for learning to write **unit tests**. Unit tests are small, automated tests that check the behavior of individual units. A unit is often, if not usually, a single function. In order to be testable a function should produce predictable results. Expected value **5**, for instance can be used to test the following function:
```js
function addTwoAndThree() {
  return 2+3;
}
```
Tape is known as the ‘bare minimum’ testing framework. As such it is lightweight, with no configuration required and free from global variables such as ‘describe.’ Tests produced with Tape are JavaScript files and can run in Node or in a browser.

Tape produces TAP output. TAP stands for Test Anything Protocol, it is documented here. It was originally designed to test Perl code in the late 1980s. A protocol is a standardised way of doing something, in case of TAP reporting the outcome of unit tests. A classic example of a protocol is meeting the Queen: call her ‘Ma’am’ (like in jam). TAP prescribes the following reporting from a test:

![tap-output](https://user-images.githubusercontent.com/18426161/46637825-cefac600-cb55-11e8-8705-3f7648c1e44f.png)

## Setting up the environment

## Your first tests
