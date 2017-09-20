# Shellestial Test Runner

> [WARNING] Please read carefully this note before using this project. It contains important information.

Content

1. What is **Shellestial Test Runner**, and when to use it ?
2. What should you know before using **Shellestial Test Runner** ?
3. How to use **Shellestial Test Runner** ?
4. Known issues
5. Miscellanous

##1. What is **Shellestial Test Runner**, and when to use it ?
**Shellestial Test Runner** is a collection of bash shell scripts that help write test suites using bash.

### Shellestial Test Runner in action

![Shellestial Test Runner started by ant](https://github.com/sporniket/shellestial/wiki/shellestial-demo-1-running.png)

![Shellestial Test Runner summary report](https://github.com/sporniket/shellestial/wiki/shellestial-demo-2-summary-report.png)

### What's in v1.0.0

* The test runner scripts.

### Roadmap

The following features are planned :

* an installable set of commands (shell scripts) to bootstrap a test suite collection and run it.
* a build procedure to get a debian package to install **Shellestial Test Runner** on any debian system.

### Licence
 **Shellestial Test Runner** is free software: you can redistribute it and/or modify it under the terms of the
 GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 option) any later version.

 **Shellestial Test Runner** is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for
 more details.

 You should have received a copy of the GNU Lesser General Public License along with **Shellestial Test Runner**.
 If not, see http://www.gnu.org/licenses/ .


## 2. What should you know before using **Shellestial Test Runner** ?
**Shellestial Test Runner** has been writen on a Ubuntu 16.04 LTS system, and thus may unknowingly rely on specificities.

> Do not use **Shellestial Test Runner** if this project is not suitable for your project.

## 3. How to use **Shellestial Test Runner** ?

### Manually bootstrap a standalone test suite collection in your project
To get the latest available code, one must clone the git repository, build and install the command.

	git clone https://github.com/sporniket/shellestial.git
	cd shellestial

In your project folder, create a ```test/suiteXxx/data``` folder, with ```Xxx``` the name of your first test suite.

  mkdir -p test/suiteXxx/data

Then copy from shellestial folder :
* ```standalone/run``` into ```test```
* ```standalone/describe``` into ```test/suiteXxx```

In the ```suiteXxx``` folder, each test are writen in a bash script with a filename starting with ```test```, e.g. ```testParameterIdIsMandatory```.

Add new test suites by creating a folder with a name starting with ```suite```, e.g. ```suiteAuthentication```

### Run a test suite of a standalone test
Invoke the run script. It is not required to be in the test folder to invoke the script.

## 4. Known issues
See the [project issues](https://github.com/sporniket/shellestial/issues) page.

## 5. Miscellanous
### Report issues
Use the [project issues](https://github.com/sporniket/shellestial/issues) page

Please report the step to reproduce an issue, the linux distribution and the bash version, at least.
