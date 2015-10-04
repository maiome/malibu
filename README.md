maiome library of utilities
=============================

[![Build Status](https://ci.maio.me/api/badge/github.com/maiome-development/malibu/status.svg?branch=master)](https://ci.maio.me/github.com/maiome-development/malibu)

This is a library of semi-useful and hopefully reusable utilities used within a few
of the projects that are in development under the maiome namespace.

config.configuration
----------------------
a "simple" config reader with section promises and special types.

connection.connection
---------------------
a structured, packet-based connection client.

connection.packets
------------------
an extensible packet implementation for use with the other connection classes.

connection.server
-----------------
a structured, packet based connection server.

database.dbmapper
-----------------
a reflective/introspective ORM used for simple object relations in SQLite (and maybe others).

database.dbtypeconv
-------------------
a series of sqlite "middlewares" to do useful type conversions.

design.borgish
--------------
a class mixin loosely based on the shared-state Borg design pattern by Alex Martelli.

design.brine
------------
a class mixin used for ORM-like serialization. usable for compressing complex objects down to
simple JSON strings for storage in a database. also provides a caching object implementation that may some day have
fuzzy search.

text.ascii
----------
map of ASCII terminal color outputs with a string wrapper.

text.table
----------
relatively simple text table formatter that allows formatting of data stored in different structures.

util (functions in `__init__.py`)
---------------------------------
series of functions that are used to perform inspection of the current frame or the caller frame.

util.args
---------
flexible command line argument parser.

util.decorators
---------------
package of generators that create decorators that can be attached to object instances or other things.

util.log
--------
logging driver that sits on top of Python's built-in logging module to simplify logger usage and provide
more informative statements by way of caller inspection

util.names
----------
simple random name generator.

util.scheduler
--------------
a simple tick-based scheduler suitable for use in ticking event loops.
now supports pluggable job stores for persisting jobs in external databases such as Redis, Riak, etc.
