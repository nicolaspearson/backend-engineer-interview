# Backend / Platform Engineer Coding Challenge

We use Typescript extensively throughout our backend codebase, however you may use any of the 
following programming languages to complete the challenge: Typescript, Javascript, Python, Java, 
Ruby, Rust, Go.

Use your README to discuss the experience you have with the technical stack you selected and we'll 
keep that in mind when reviewing your solution.

## Challenge

We have a list of ordered integers (e.g.: `[1, 3, 7, 8, 9, 10, 11]`). Suppose we slice that list 
at a random index and append the "top" half of list to the "bottom" (maintaining the order of both 
halves while doing so).

1. Write a function that returns the largest integer in the "shifted" list.

    View the samples below for a better understanding of how the lists are mutated:
    ```typescript
    // Sample 1
    const initialList = [1, 3, 7, 8, 9, 10, 11]  // Here is our initial ordered list
    const shiftedList = [8, 9, 10, 11, 1, 3, 7]  // Here is the list after it has been sliced (at index 3) and shifted
    // Your function should return `11`

    // Sample 2
    const initialList = [2, 4, 6, 8, 10]  // Here is our initial ordered list
    const shiftedList = [6, 8, 10, 2, 4]  // Here is the list after it has been sliced (at index 2) and shifted
    // Your function should return `10`

    // Sample 3
    const initialList = [2, 4, 6, 8, 10]  // Here is our initial ordered list
    const shiftedList = [2, 4, 6, 8, 10]  // Here is the list after it has been sliced (at index 0) and shifted
    // Your function should return `10`
    ```
    - Can you identify any edge cases that we need to account for?
    - Can you explain the orders of growth implications of the algorithm you implemented?
    - Suppose our initial list contains 1 million elements, is there a more performant way we can 
    find the answer?

2. Write unit tests for your code.
3. Create a github action that will run the unit tests (the pipeline should be green if the tests 
pass and red if one or more of the tests fail).

### Time Allotment

We respect your time and don't want you spending more than 8 hours on the challenge (The challenge 
is scoped for a ~3hr time-frame). We just want to get a sense of your thought process and development 
patterns. If there are features you don't have time to implement, feel free to use pseudo code to 
describe the intended behavior.

### Your Challenge README

Include the following items in your README:

- A description of the problem and solution.
- How we can run your solution locally.
- The reasoning behind your technical decisions, e.g. trade-offs you might have made, anything you left out, 
or what you might do differently if you were to spend additional time on the challenge.

### Commit History

You may use whichever development workflow works best for you. If your solution is small enough for 
a single commit, that is fine, we just ask that you keep your [commit history as clean as possible](https://www.notion.so/Keeping-Commit-Histories-Clean-0f717c4e802c4a0ebd852cf9337ce5d2).

## What We Review

The aspects of your solution we will be reviewing:

- **Clarity**: Does the README clearly explain the problem and solution?
- **Correctness**: Does the application do what was asked? If there is anything missing, does the README explain why it is missing?
- **Code Quality**: Is the code simple, easy to understand, and maintainable?
- **Testing**: How thorough are the automated tests?
- **Technical Choices**: Do the choices of architecture, libraries, etc. seem appropriate for the challenge?
