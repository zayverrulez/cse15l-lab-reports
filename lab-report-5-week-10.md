# Week 10 Lab Report 5


Explain:
* How you found the tests with different results (Did you use vimdiff on the
results of running a bash for loop? Did you search through manually? Did you
use some other programmatic idea?)
    * To find the tests with different results, I used vimdiff to open up the two files of results from the MarkdownParse on the test-files/ made previously. These two files have the results of running the bash file with a for loop that includes the name of the MarkDownParse file, the iteration/testfile and results.

Done from lab 9 as navigator/driver with lab partners.

---

## Differing Test 1
* Provide a link to the test-file with different-results (in the provided repository or
your repository , either is fine)
    * [Link - Click me!](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md)
* Describe which implementation is correct, or neither if both give the wrong output
    * Implementation test-file 194 is wrong for both, they have wrong outputs. See below in next point.
* Indicate both actual outputs (provide screenshots) and also what the expected output is (list the links that are expected in the output).
    * Both MarkdownParses fail this test-file. The correct expected output for the file is: `[my(url)]`.
    * Wrong inputs: ![Wrong Inputs](lab-report-5-photos\Screenshot_1.png)

* For the implementation that’s not correct (or choose one if both are incorrect), describe the bug (the problem in the code) in about 2-3 sentences. You don’t have to provide a fix, but you should be specific
about what is wrong with the program, and show the code that should be fixed (Provide a screenshot of code and highlight where the change needs to be made).
    * The below pictured part of the code causes this symptom. It includes whatever is found between the pair of secondary closed parentheses. Therefore, the output `[url]` as it was included in the parentheses but not the actual link. 
    * Picture: ![Picture](lab-report-5-photos\Screenshot_3.png)

---

## Differing Test 2
* Provide a link to the test-file with different-results (in the provided repository or
your repository , either is fine)
    * [Link - Click me!](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md)
* Describe which implementation is correct, or neither if both give the wrong output
    * My MarkdownParse got it right: `[]`, empty brackets with no link. The given MarkdownParse got it wrong, see picture below.
* Indicate both actual outputs (provide screenshots) and also what the expected output is (list the links that are expected in the output).
    * Outputs: ![Outputs](lab-report-5-photos\Screenshot_2.png)

* For the implementation that’s not correct (or choose one if both are incorrect), describe the bug (the problem in the code) in about 2-3 sentences. You don’t have to provide a fix, but you should be specific
about what is wrong with the program, and show the code that should be fixed (Provide a screenshot of code and highlight where the change needs to be made).
    * The third line in the picture does not check for other factors which invalidate a link before adding the text between the found parentheses. Though similar to the previous flaw, its difference lies in the '<' and '>'characters. This bug does not seem to be solvable with one change.
    * Picture: ![Picture](lab-report-5-photos\Screenshot_4.png)