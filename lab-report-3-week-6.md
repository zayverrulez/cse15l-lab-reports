# Week 6 Lab Report 3

Hello! I tested positive for COVID this last week and have been in University Isolation Housing, missing the last two labs in person. However, I still made a lot of effort to remotely join and work with my lab partners on these two labs. Thankfully, due to the pair programming/driver navigator structure of the labs, I was able to utilize my full presense with remote tools like Discord and Zoom while not being physically present.

---

## Streamlining ssh Configuration

 This is really helpful because it allows you to connect to your remote computer through SSH much faster and more efficently. By making a config file in the ~/.ssh directory you can streamline the amount of commands required to connect. Now instead of having to remember your username, you can just remember which host your are trying to connect to.

* Show your .ssh/config file, and how you edited it (with VScode, another program, etc)

    * ![Picture 1.1](lab-report-3-photos\Screenshot_3.png)
* Show the ssh command logging you into your account using just the alias you chose.

    * ![Picture 1.2](lab-report-3-photos\Screenshot_1.png)
* Show an scp command copying a file to your account using just the alias you chose.

    * ![Picture 1.3](lab-report-3-photos\Screenshot_4.png)

---

## Setup Github Access from ieng6

This allows you to interact with Github and your remote computer in a new different way. It allows for the simplication of certain workflows because of this new more direct and therefore "cleaner" connection.

* Show where the public key you made is stored on Github and in your user account (screenshot).

    * ![Picture 2.1](lab-report-3-photos\Screenshot_16.png)

* Show where the private key you made is stored on your user account (but not its contents) as a screenshot.

    * ![Picture 2.2](lab-report-3-photos\Screenshot_15.png)

* Show running git commands to commit and push a change to Github while logged into your ieng6 account.

    * ![Picture 2.3.2](lab-report-3-photos\Screenshot_14.png)

* Show a link for the resulting commit.

    * [https://github.com/zayverrulez/markdown-parser/commit/42c2beae7280482fdb299b5d69023e3d41c06c25](https://github.com/zayverrulez/markdown-parser/commit/42c2beae7280482fdb299b5d69023e3d41c06c25)


---

## Copy whole directories with ```scp -r```

Things get a little weird when you copy whole directories. By weird, I mean abnormal--not expected for those who are like me and just learning. Using a -r recursive arguments allows you to get it done.

* Show copying your whole markdown-parse directory to your ieng6 account.

    * ![Picture 3.1.1](lab-report-3-photos\Screenshot_17.png)
    * ![Picture 3.1.2](lab-report-3-photos\Screenshot_18.png)
    * ![Picture 3.1.3](lab-report-3-photos\Screenshot_19.png)

* Show logging into your ieng6 account after doing this and compiling
and running the tests for your repository.

    * ![Picture 3.2](lab-report-3-photos\Screenshot_5.png)

* Show (like in the last step of the first lab) combining scp, ;, and ssh to copy the whole directory and run the tests in one line.

    * ``` scp -r markdown-parser ieng6:~/markdown-parser ; ssh ieng6 "cd markdown-parser;/software/CSE/oracle-java-17/jdk-17.0.1/bin/javac -cp .:lib/* *.java;/software/CSE/oracle-java-17/jdk-17.0.1/bin/java -cp .:lib/* org.junit.runner.JUnitCore MarkdownParseTest" ```
    * ![Picture 3.3.1](lab-report-3-photos\Screenshot_6.png)
    * ![Picture 3.3.2](lab-report-3-photos\Screenshot_7.png)
    * ![Picture 3.3.3](lab-report-3-photos\Screenshot_8.png)
    * ![Picture 3.3.4](lab-report-3-photos\Screenshot_9.png)