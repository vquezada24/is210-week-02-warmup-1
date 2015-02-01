#####################
IS 210 Assignment #02
#####################
*************
Warm-Up Tasks
*************

:College: CUNY School of Professional Studies
:Course-Name: Software Application Programming I
:Course-Code: IS 210
:Lesson: 02
:Points: 12
:Due-Date: YYYY-MM-DDTHH:mm:ss

Overview
========

The warm-up tasks this week will focus on general git repository tasks. You'll
be tasked to manipulate files with git's tools prior to submitting the work
through the git pull request workflow.

Instructions
============

The following tasks will either have you interacting with existing files in
the assignment repository or creating new ones on the fly. Don't forget to add
your interpreter directive, utf-8 encoding, and a short docstring with any new
files that you create!

.. important::

    In these exercises, you may, on occasion, come across a task that requres
    you to research or use a function or method not directly covered by the
    course text. Since Python is such a large language it would be impossible
    for the author to have included descriptions of each and every available
    function which would largely duplicate the offical Python documentation.

    A *vital* skill to successful programming is being comfortable searching
    for and using official language documentation sources like the
    `Python String Documentation`_ page. Throughout our coursework we will be
    practicing both the use of the language in practice and the search skills
    necessary to become functional programmers.

Warm-Up Tasks
=============

Task 01
-------

We'll start by creating a new file and adding it to our repository.

Specifications
^^^^^^^^^^^^^^

1.  Create a new file named ``task_01.txt`` in the root of your repository. You
    can use ``idle`` to create a new file by typing the file's name after the
    ``idle`` command such as:

    .. code:: console

        $ idle somefile

    .. tip::

        While ``idle`` will likely be the main tool for many of you, you
        could also use the ``touch`` command to achieve the same objective.

2.  Use ``git status`` to check that git sees your unstaged file.

3.  Use the ``git add`` command to add this file to staging for the next
    commit.

4.  Use ``git status`` to check that your changes are properly staged for
    committing.

5.  Use ``git commit`` to commit your change into the repository.

Task 02
-------

For task 02, you'll be making a small change to an existing file.

Specifications
^^^^^^^^^^^^^^

1.  Open the file, ``task_02.py`` with your ``idle`` python editor.

2.  Replace the name ``Snoopy`` with your own name.

    .. tip::

        Since this is a Python file, you can test to see if you made the
        right change by running your python file in idle or on the command
        line.

3.  Use ``git status`` to check that git sees your unstaged file.

4.  Use the ``git add`` command to add this file to staging for the next
    commit.

5.  Use ``git status`` to check that your changes are properly staged for
    committing.

6.  Use ``git commit`` to commit your change into the repository.

Task 03
-------

For our third warm-up exercise, we'll move a file with ``git mv`` to retain
the history of the file. When renaming or moving files in Git, it's important
to use ``git mv`` and not other tools that rename files or folders as Git
could lose track of file history if done incorrectly.

Specifications
^^^^^^^^^^^^^^

1.  Use ``git mv`` to rename the file, ``Task 3.py`` to ``task_03.py``.

    .. hint::

        As you'll quickly discover, having spaces in file names on the console
        can be a pain in the neck! Either encapsulate the file name with
        quotation marks (eg, ``"some file.txt"``) or try *escaping* the space
        with a backslash (``some\ file.txt``).

2.  Use ``git status`` to check that your changes are properly staged for
    committing.

3.  Use ``git commit`` to commit your change into the repository.

.. note::

    Did you notice how you didn't have to use ``git add`` this time around?
    Some Git commands that interact with files already under version control
    don't require you to add the changes to the repository and are
    automatically staged.

Task 04
-------

The last in our quartet of major operations in git is removing (aka *deleting*)
a file in Git. As you'll see in this exercise, removing a file and a directory
are not exactly the same.

Specifications
^^^^^^^^^^^^^^

1.  Use the ``git rm`` to remove the single file, ``task_04.txt``

2.  Use ``git rm`` to remove the directory ``task_04`` and all of the files
    contained within it.

    .. hint::

        Look into what the ``-r`` or recursive flag does to modify how
        ``git rm`` works.

3.  Use ``git status`` to check that your changes are properly staged for
    committing.

4.  Use ``git commit`` to commit your change into the repository.

Task 05
-------

As we discussed in the *Concepts and Terms* document, executable Python files
should have an interpreter directive. One such file in our repository happens
to be missing one!

Specifications
^^^^^^^^^^^^^^

1.  Edit ``task_05.py`` and add an interpreter directive in the proper
    location.

2.  Use ``git status`` to check that git sees your unstaged file.

3.  Use the ``git add`` command to add this file to staging for the next
    commit.

4.  Use ``git status`` to check that your changes are properly staged for
    committing.

5.  Use ``git commit`` to commit your change into the repository.

Executing Tests
===============

Code must be functional and pass tests before it will be eligible for credit.

Task 06
-------

The encoding statement is as, if-not more, important to add to your Python
files than your interpreter directive. As it happens, one of our files
happens to be missing its coding statement. Correct it to receive credit
for this task.

Specifications
^^^^^^^^^^^^^^

1.  Edit ``task_06.py`` and add an coding statement in the appropriate
    location.

2.  Use ``git status`` to check that git sees your unstaged file.

3.  Use the ``git add`` command to add this file to staging for the next
    commit.

4.  Use ``git status`` to check that your changes are properly staged for
    committing.

5.  Use ``git commit`` to commit your change into the repository.

Executing Tests
===============

Code must be functional and pass tests before it will be eligible for credit.

Linting
-------

Lint tests check your code for syntactic or stylistic errors To execute lint
tests against a specific file, simply open a terminal in the same directory as
your code repository and type:

.. code:: console

    $ pylint filename.py

Where ``filename.py`` is the name of the file you wish to lint test.

Unit Tests
----------

Unit tests check that your code performs the tested objectives. Unit tests
may be executed individually by opening a terminal in the same directory as
your code repository and typing:

.. code:: console

    $ nosetests tests/name_of_test.py

Where ``name_of_test.py`` is the name of the testfile found in the ``tests``
directory of your source code.

Running All Tests
-----------------

All tests may be run simultaneously by executing the ``runtests.sh`` script
from the root of your assignment repository. To execute all tests, open a
terminal in the same directory as your code repository and type:

.. code:: console

    $ sh runtests.sh

Submission
==========

Code should be submitted to `GitHub`_ by means of opening a pull request.

As-of Lesson 02, each student will have a branch named after his or her
`GitHub`_ username. Pull requests should be made against the branch that
matches your `GitHub`_ username. Pull requests made against other branches will
be closed.  This work flow mimics the steps you took to open a pull request
against the ``pull`` branch in Week Two.

For a refresher on how to open a pull request, please see homework instructions
in Lesson 01. It is recommended that you run PyLint locally after each file
is edited in order to reduce the number of errors found in testing.

In order to receive full credit you must complete the assignment as-instructed
and without any violations (reported in the build status). There will be
automated tests for this assignment to provide early feedback on program code.

When you have completed this assignment, please post the link to your
pull request in the body of the assignment on Blackboard in order to receive
credit.

.. _GitHub: https://github.com/
.. _Python String Documentation: https://docs.python.org/2/library/stdtypes.html
