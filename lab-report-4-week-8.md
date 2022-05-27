# Week 8 Lab Report 4

## Repo Links

* A link to your markdown-parse repository in week 7
    * [https://github.com/zayverrulez/markdown-parser](https://github.com/zayverrulez/markdown-parser)
* A link to the one you reviewed in week 7
    * [https://github.com/szreik/markdown-parser](https://github.com/szreik/markdown-parser)

---

## Tests

### Snipet Test 1

* Decide on what it should produce (i.e., expected output) by using either VScode preview or the CommonMark demo site
    * Expected output: ```[`google.com, google.com, ucsd.edu]```
    * VScode preview: ![Screenshot 1](lab-report-4-photos\Screenshot_1.png)
* Showing the code in MarkdownParseTest.java for how you turned it into a test
    * ![Screenshot 5](lab-report-4-photos\Screenshot_5.png)
* For your implementation, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.
    * My repo: failed. ![My repo](lab-report-4-photos\Screenshot_8.png)
* For the implementation you reviewed in Week 7, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.
    * infinite loop ![Review repo](lab-report-4-photos\Screenshot_11.png)

### Snipet Test 2

* Decide on what it should produce (i.e., expected output) by using either VScode preview or the CommonMark demo site
    * Expected output: ```[a.com, a.com(()), example.com]```
    * VScode preview: ![Screenshot 1](lab-report-4-photos\Screenshot_2.png)
* Showing the code in MarkdownParseTest.java for how you turned it into a test
    * ![Screenshot 6](lab-report-4-photos\Screenshot_6.png)
* For your implementation, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.
    * My repo: failed. ![My repo](lab-report-4-photos\Screenshot_9.png)
* For the implementation you reviewed in Week 7, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.
    * infinite loop ![Review repo](lab-report-4-photos\Screenshot_11.png)

### Snipet Test 3

* Decide on what it should produce (i.e., expected output) by using either VScode preview or the CommonMark demo site
    * Expected output: ```[https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule]```
    * VScode preview: ![Screenshot 1](lab-report-4-photos\Screenshot_3.png)
* Showing the code in MarkdownParseTest.java for how you turned it into a test
    * Review repo: infinite loop ![Screenshot 7](lab-report-4-photos\Screenshot_7.png)
* For your implementation, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.
    * Failed. ![My repo](lab-report-4-photos\Screenshot_10.png)
* For the implementation you reviewed in Week 7, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.
    * infinite loop ![Review repo](lab-report-4-photos\Screenshot_11.png)

---

## Responses to Questions

* Answer the following questions with 2-3 sentences each:
    * Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.
        * Answer
    * Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.
        * Answer
    * Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.
        * Answer
* If your code already works on some/all test cases, include an explanation of what were the code changes that allowed the tests to pass.
