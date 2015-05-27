Git Starter Guide
=================

Git Features
------------

Git and SVN differences
~~~~~~~~~~~~~~~~~~~~~~~

- Git is much faster than Subversion​
- Subversion allows you to check out just a subtree of a repository; Git requires you to clone the entire repository (including history) and create a working copy that mirrors at least a subset of the items under version control.​
- Git's repositories are much smaller than Subversions (for the Mozilla project, 30x smaller)​
- Git was designed to be fully distributed from the start, allowing each developer to have full local control​
- Git branches are simpler and less resource heavy than Subversion's​
- Git branches carry their entire history​
- Merging in Git does not require you to remember the revision you merged from (this benefit was obviated with the release of Subversion 1.5)​
- Git provides better auditing of branch and merge events​
- Git's repo file formats are simple, so repair is easy and corruption is rare.​

Git major features over subversion
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- Distributed Nature​
- Access Control​
- Branch Handling
- Performance (Speed of Operation)​
- Smaller Space Requirements

Using Puttygen
--------------

Purpose
~~~~~~~
Puttygen is a tool that you can use to convert private keys into different formats.
You can also use this tool to generate a public key from a given private key.

Convert Private Key
~~~~~~~~~~~~~~~~~~~
You will receive a private key from JP that is using the RSA format. In order to use it in Tortoisegit, you need to convert it to OpenSSH format first. 

The following illustrates the steps:

- Open puttgen

.. figure:: _static/puttygen1.png
    :align: center

- Go to File, then "Load Private Key"
	
.. figure:: _static/puttygen2.png
    :align: center

.. figure:: _static/puttygen3.png
    :align: center

.. figure:: _static/puttygen4.png
    :align: center

.. figure:: _static/puttygen5.png
    :align: center

.. figure:: _static/puttygen6.png
    :align: center	
	
	