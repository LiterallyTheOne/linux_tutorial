pwd, ls
=======

There two commands are two of the most basic commands
in linux.
They are being frequently by so many people.
Their usage can be summarized by below:

* ``pwd``: To find out where you are
* ``ls``: To find out the content of the current directory

In these tutorial we discuss about these two commands.

pwd
---

``pwd`` stands for **Print Working Directory**.
And by the sounds of it, it prints the current
directory. for example if we are right now in
``/home/ramin`` (ramin is my name by the way)
the result of typing ``pwd`` in terminal and pressing
enter would be: ``/home/ramin``

ls
--

``ls`` stands for **List**.
If you write it with no arguments,
it lists the current directory's
content.
It can get an argument that shows the content
of the given directory.
For example if you type ``ls`` in a directory that
has structure like below:

.. code-block:: text

    .
    ├── directory_test_1
    │   ├── directory_test_3
    │   └── file_test_4.txt
    ├── directory_test_2
    ├── file_test_1.txt
    └── file_test_2.txt

the output of ``ls`` would be:

.. code-block::

    directory_test_1  directory_test_2  file_test_1.txt  file_test_2.txt


