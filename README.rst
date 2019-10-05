README
======

``island-lab-competition-tools`` is a toolset including:

* a puzzle generator
* a puzzle resolver runner

Generator Using Example
-----------------------

The next command will attempt to generate 10 batches with 100 tasks in each::

    ./island-lab-generator \
            ../../island-lab.proj/island-lab.BUILD/bin/island-lab-resolver \
            6 5 4 \
            10 100 \
            ../tasks.txt

The result list will highly probably be dramatically less (or even empty!)
then was ordered, because of skipped failure attempts.

Runner Using Example
--------------------

To run resolver with generated tasks::

    ./island-lab-runner \
            ../../island-lab.proj/island-lab.BUILD/bin/island-lab-resolver \
            ../tasks.txt \
            ../out-full.txt ../out-problem.txt
