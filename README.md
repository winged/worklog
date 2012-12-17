About this script
=================

This is a small python script that helps you track what you're currently
working on.

It helps you remember what you did all day (or night), then helps you
with reconstructing your work day. No fancy GUI or anything, just a
commandline thingy that intends to be useful, yet simple.

How to use
==========

Install the script in your ~/bin or /usr/local/bin folder and chmod+x
it. Then, you can issue the following commands to track your work:

    work on <task-description>     -- start working on given task description, stop any previous task
    work edit <task-description>   -- edits text of last task
    work done                      -- stop current task
    work resume                    -- resumes the last logged task
    work resume <id>               -- resumes task with given id (see work since, work today etc.)
    work reset                     -- removes last task

There are also a few commands available to list / analyze what you've
done in the past:

    work today                     -- list all tasks recorded today
    work list                      -- list all recorded tasks
    work since yyyy-mm-dd          -- list all tasks since the given date
    work sum                       -- Sum of work time, grouped by day

Yep, that's about it.

Files
=====

The script stores it's data in an SQLite database in your home directory
under ~/.workon/worklog.db.
