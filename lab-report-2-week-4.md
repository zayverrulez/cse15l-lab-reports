# Week 4 Lab Report 2

Hello! Please note that for this lab we used the pair-programming method, and my lab partner Kasey was the designated driver. This means that although I have very similar code examples, we mainly worked on his repository as the instructions dictated. Thanks and good luck grading!

---

## 1st code change to fix a bug

* Show a screenshot of the code change diff from Github

    * ![Image](lab-report-2-photos\screencapture-github-zayverrulez-markdown-parser-commit-535ea718011a88ef2952324682ae1341ea2a8013-2022-04-24-21_44_30.png)

* Link to the test file for a failure-inducing input that prompted you to make that
change

    * *I am confused by the word "link", as it is a little vauge how I should "link" to this failure-inducing input. Nevertheless, here is an actual GitHub link to the input test file that caused this, and a photo. I am doing this in the hope to please all possible expecting outcomes.*

        * [Link to failure-inducing input test file](https://github.com/zayverrulez/markdown-parser/blob/main/test-file3.md)

        * Photo of failure-inducing input test file

            ![Image](lab-report-2-photos\Screenshot_5.png)

* Show the symptom of that failure-inducing input by showing the output of
running the file at the command line for the version where it was failing (this
should also be in the commit message history)
    * My own personal example with different links.
      ```
      [https://vimeo.com,https://lh3.googleusercontent.com/2hDpuTi-0AMKvoZJGd-yKWvK4tKdQr_kLIpB_qSeMau2TNGCNidAosMEvrEXFO9G6tmlFlPQplpwiqirgrIPWnCKMvElaYgI-HiVvXc=w600, https://youtube.com]
      ```
    * A photo from my pair programming driver partner's output:
    ![Kasey's output](lab-report-2-photos\Screenshot_4.png)

* Write 2-3 sentences describing the relationship between the bug, the
symptom, and the failure-inducing input.

    * The bug is that the code is not looking for an "!" before the open bracket. The symptom is that pictures in the markdown file are treated like links and are put in the link list. The failure-inducing input is `test-file3.md` which contains a picture between two links. 

---

## 2nd code change to fix a bug

* Show a screenshot of the code change diff from Github

    * ![Image](lab-report-2-photos\Screenshot_7.png)

* Link to the test file for a failure-inducing input that prompted you to make that
change

    * *I am confused by the word "link", as it is a little vauge how I should "link" to this failure-inducing input. Nevertheless, here is an actual GitHub link to the input test file that caused this, and a photo. I am doing this in the hope to please all possible expecting outcomes.*

        * [Link to failure-inducing input test file](https://github.com/zayverrulez/markdown-parser/blob/main/test-file4.md)

        * Photo of failure-inducing input test file

            ![Image](lab-report-2-photos\Screenshot_3.png)

* Show the symptom of that failure-inducing input by showing the output of
running the file at the command line for the version where it was failing (this
should also be in the commit message history)
    * Index is at 0 and then asked to go to -1 which is out of bounds.
      ```
      Exception in thread "main" java.lang.IndexOutOfBoundsException: Index: 0
      ```

* Write 2-3 sentences describing the relationship between the bug, the
symptom, and the failure-inducing input.

    * The bug is that the program does not account for instances where links are the first thing in the markdown file. The symptom is that the problem throws an exception. The failure-inducing input is test-file5.md, previously test-file3.md where the link is first in the file.

---

## 3rd code change to fix a bug

* Show a screenshot of the code change diff from Github

    * ![Image](lab-report-2-photos\Screenshot_7.png)

* Link to the test file for a failure-inducing input that prompted you to make that
change

    * *I am confused by the word "link", as it is a little vauge how I should "link" to this failure-inducing input. Nevertheless, here is an actual GitHub link to the input test file that caused this, and a photo. I am doing this in the hope to please all possible expecting outcomes.*

        * [Link to failure-inducing input test file](https://github.com/zayverrulez/markdown-parser/blob/main/test-file4.md)

        * Photo of failure-inducing input test file

            ![Image](lab-report-2-photos\Screenshot_3.png)

* Show the symptom of that failure-inducing input by showing the output of
running the file at the command line for the version where it was failing (this
should also be in the commit message history)
    * My own personal example with different links.
      ```
      [https://vimeo.com,https://lh3.googleusercontent.com/2hDpuTi-0AMKvoZJGd-yKWvK4tKdQr_kLIpB_qSeMau2TNGCNidAosMEvrEXFO9G6tmlFlPQplpwiqirgrIPWnCKMvElaYgI-HiVvXc=w600, https://youtube.com]
      ```
    * A photo from my pair programming driver partner's output:
    ![Kasey's output](lab-report-2-photos\Screenshot_4.png)

* Write 2-3 sentences describing the relationship between the bug, the
symptom, and the failure-inducing input.

    * The bug is that the code is not looking for an "!" before the open bracket. The symptom is that pictures in the markdown file are treated like links and are put in the link list. The failure-inducing input is `test-file3.md` which contains a picture between two links. 