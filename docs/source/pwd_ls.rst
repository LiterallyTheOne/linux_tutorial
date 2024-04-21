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

There are some important options for ls that we are
going to discuss some of them in further.

option -a
^^^^^^^^^

``-a`` stands for all.
When we use this option, it shows all the files
despite being hidden or not.
For example if we have a hidden file in the
directory's structure above with the name of
``.hidden_file_1.txt`` the output of ``ls -a``
would be:

.. code-block:: text

    .  ..  directory_test_1  directory_test_2  file_test_1.txt  file_test_2.txt  .hidden_file_1.txt

Which ``.`` represents the current directory, ``..``
represents the parent directory.

option -l
^^^^^^^^^

``-l`` stands for ``long``.
If you use this option, it shows all the files
with some extra details.
Including file permissions, number of links to this file,
owner, group, size in bytes, creation date, name.
for example one the output of ``ls -l`` can be:

.. code-block:: text

    total 8
    drwxr-xr-x 3 ramin ramin 4096 Mar 16 12:00 directory_test_1
    drwxr-xr-x 2 ramin ramin 4096 Mar 16 12:00 directory_test_2
    -rw-r--r-- 1 ramin ramin    0 Mar 16 11:59 file_test_1.txt
    -rw-r--r-- 1 ramin ramin    0 Mar 16 11:59 file_test_2.txt



