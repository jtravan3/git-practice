# The best way to 'git' something is by practice!

## Overview

This repository contains the needed base code and instructions for someone who is interested in learning or improving their `git` and Github skills. 

## Usage

This repository is designed so that anyone who is wanting to learn git or practice their git skills can do the following:

1.) Clone the repository to their local machine
2.) Make changes to files in the repository
3.) Commit those changes to a new branch named `feature/{githubUsername}`
4.) Push the branch to the repository
5.) Open a pull request on [Github](https://github.com/jtravan3/git-practice)

## IDE (IntelliJ)

I use the IDE IntelliJ for all coding examples. You can use any IDE that you choose (Eclipse, Netbeans, VS Code, etc.) however,
I will only be able provide assistance for IntelliJ.

IntelliJ is quite expensive however students/instructors can receive a free license by filling out an application with their
school email address. Simply go to [https://www.jetbrains.com/student/](https://www.jetbrains.com/student/) and fill out an
application in order to receive your free license.

## Git Practice

If you're interested in getting started with `git`, follow the instructions below to help you understand the process.

### Git Command Line

1.) First you will need the `git` command line tools. Download `git` located at [https://git-scm.com/](https://git-scm.com/).

2.) Install maven 3.6.0 and Java JDK 11. JDK located at [https://openjdk.java.net/install/](https://openjdk.java.net/install/). If you have a Mac you can use `brew`.

```bash
brew install maven
brew install java
```

3.) Clone down the repository from Github

```bash
git clone git@git.github.com:jtravan3/git-practice.git
```

4.) Build the project

```bash
mvn clean install
```

You should see a success if everything is set up correctly. You should be able to run the `HelloWorld` program successfully if you have everything setup correctly.

5.) Now that you have your environment setup we'll want to make some changes to some files. For this repository you're going to make two changes. One will be a version change in
`pom.xml` and the second will be an entry in `CHANGELOG.md`.

6.) Navigate to `pom.xml` and increase the minor fix version by one. See the before and after example below.

Before
```xml
<groupId>edu.citadel</groupId>
<artifactId>git-practice</artifactId>
<version>1.0.1</version>
```

After
```xml
<groupId>edu.citadel</groupId>
<artifactId>git-practice</artifactId>
<version>1.0.2</version>
```

7.) Next navigate to `CHANGELOG.md` and add an entry for yourself. See the example below

```markdown
## [1.0.1] - 2019/12/11

### Added

- John Ravan updated the version to 1.0.1
```

8.) After completing the file edits within your repository create a branch for the change

```bash
git checkout -b feature/{githubUsername}
```

9.) Add all of your changed files to the newly created branch

```bash
git add .
```

10.) Commit all of the added files to your branch with a message

```bash
git commit -m "I added myself to the CHANGELOG.md"
```

11.) Now that all of your changes have been commit to the new branch, push the new branch to the remote repository.

```bash
git push origin feature/{githubUsername}
```

12.) Visit the repository through [Github](https://github.com/jtravan3/git-practice) and open a pull request for merging your feature branch into
the `master` branch. From here, I'll review the pull request to make sure it looks great and then merge it in. You'll be added to the history of the `CHANGELOG.md`!

### Git GUI (IntelliJ)

1.) First you will need the IntelliJ IDE located at [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/). Download and install.

2.) Install maven 3.6.0 and Java JDK 11. JDK located at [https://openjdk.java.net/install/](https://openjdk.java.net/install/). If you have a Mac you can use `brew`.

```bash
brew install maven
brew install java
```

3.) Clone down the repository from Github

```bash
git clone git@git.github.com:jtravan3/git-practice.git
```

4.) Build the project

```bash
mvn clean install
```

You should see a success if everything is set up correctly. You should be able to run the `HelloWorld` program successfully if you have everything setup correctly.

5.) Now that you have your environment setup we'll want to make some changes to some files. For this repository you're going to make two changes. One will be a version change in
`pom.xml` and the second will be an entry in `CHANGELOG.md`.

6.) Navigate to `pom.xml` and increase the minor fix version by one. See the before and after example below.

Before
```xml
<groupId>edu.citadel</groupId>
<artifactId>git-practice</artifactId>
<version>1.0.1</version>
```

After
```xml
<groupId>edu.citadel</groupId>
<artifactId>git-practice</artifactId>
<version>1.0.2</version>
```

7.) Next navigate to `CHANGELOG.md` and add an entry for yourself. See the example below

```markdown
## [1.0.1] - 2019/12/11

### Added

- John Ravan updated the version to 1.0.1
```

8.) After completing the file edits within your repository create a branch for the change

```bash
git checkout -b feature/{githubUsername}
```

9.) Add all of your changed files to the newly created branch

```bash
git add .
```

10.) Commit all of the added files to your branch with a message

```bash
git commit -m "I added myself to the CHANGELOG.md"
```

11.) Now that all of your changes have been commit to the new branch, push the new branch to the remote repository.

```bash
git push origin feature/{githubUsername}
```

12.) Visit the repository through [Github](https://github.com/jtravan3/git-practice) and open a pull request for merging your feature branch into
the `master` branch. From here, I'll review the pull request to make sure it looks great and then merge it in. You'll be added to the history of the `CHANGELOG.md`!
