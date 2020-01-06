Family Tree
-------------
My approach for this problem is Object oriented way rather than single file script.
So i made each member as a object and that object has the many family relation.
we will call all relation based on that particular member level rather than family
level.

Initial Loading
---------------
I am giving python Dict as a initial loading data. It is very easy to port to Json/Yaml
since i can only provide one command line input i am not doing here.

Layered Approach
---------------
I am generating all programmer specific output at the end of return calls using
a decorator
Please check utils.py/format_output decorator



*** UPDATE***

Build
----------------
Adds setup.py file for automate testing
User only need to type *python setup.py* test to run the unit test
This will install the pytest package and run unit test

Unit Test (Code coverage > 90%)
-------------
I have used pytest module. Since we can write tests with much easily
https://pythontesting.net/transcripts/2-pytest-vs-unittest-vs-nose/

to run: python setup.py test

Project Structure:
-------------
Made project as in proper structure, Added import in __init__.py file for better readabilty.(src/__init__.py)
Family:
    README
    geektrus.py
    setup.py
    src:
        modules
    test:
        unit_tests

Modular/Extensibility
-------------
Made functions as much as modular,
User can load different tree structure without changing the  code.
Only need to add the family tree on src/family_tree_structure.py file. as below format

{"name":"family_name",
 "members":[{"name", "sex", "mother_name", spouse"},
            .............           
           ]
}


Note:
-----------
I think I am over killing the problem to get more badges. Please give me appropriate feedback to
improve my skill







