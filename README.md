# Python project for check for and emailing out data.
# Classification (U)

# Description:
  Used to receive text input and pushes it into sendmail.  Will only send if there is data in the text input.  This program is typically used in conjunction with other project programs.


###  This README file is broken down into the following sections:
  * Features
  * Prerequisites
  * Installation
  * Program Help Function
  * Testing
    - Unit


# Features:
  * Email data received from standard in.
  * Email data from an ASCII text file.
  * Ensure there is data sent to the program, otherwise ignore request.

# Prerequisites:

  * List of Linux packages that need to be installed on the server.
    - git
    - python-pip

  * Local class/library dependencies within the program structure.
    - lib/gen_class
    - lib/arg_parser
    - lib/gen_libs


# Installation:

Install these programs using git.
  * Replace **{Python_Project}** with the baseline path of the python program.

```
umask 022
cd {Python_Project}
git clone git@github.com:deepcoder42/cond-mail.git
```

Install/upgrade system modules.

```
cd cond-mail
sudo bash
umask 022
pip install -r requirements.txt --upgrade
exit
```

Install supporting classes and libraries.

```
pip install -r requirements-python-lib.txt --target lib
```


# Program Help Function:

  All of the programs, except the command and class files, will have an -h (Help option) that will show display a help message for that particular program.  The help message will usually consist of a description, usage, arugments to the program, example, notes about the program, and any known bugs not yet fixed.  To run the help command:
  * Replace **{Python_Project}** with the baseline path of the python program.

```
{Python_Project}/cond-mail/cond_mail.py -h
```


# Testing:

# Unit Testing:

### Installation:

Install these programs using git.
  * Replace **{Python_Project}** with the baseline path of the python program.
  * Replace **{Branch_Name}** with the name of the Git branch being tested.  See Git Merge Request.

```
umask 022
cd {Python_Project}
git clone --branch {Branch_Name} git@github.com:deepcoder42/cond-mail.git
```

Install/upgrade system modules.

```
cd cond-mail
sudo bash
umask 022
pip install -r requirements.txt --upgrade
exit
```

Install supporting classes and libraries.

```
pip install -r requirements-python-lib.txt --target lib
```

# Testing:
  * Replace **{Python_Project}** with the baseline path of the python program.

```
cd {Python_Project}/cond-mail
test/unit/cond_mail/unit_test_run.sh
```

### Code coverage:

```
cd {Python_Project}/cond-mail
test/unit/cond_mail/code_coverage.sh
```

