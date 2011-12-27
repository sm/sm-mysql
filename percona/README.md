# SM Framework Percona MySQL Extension

## Prerequisites

First ensure that gcc version 4.2.1 or later along with readline and it's
development headers and the bison tool are all installed.
On an rpm based system this is typically done with:

    yum install -y gcc bison make readline readline-devel

The cmake tool is required before being able to install mysql (in
addition to the standard gcc tool chain) You can install cmake using the
SM Framework tools extension set as follows:

    sm set install tools
    sm cmake install

## Installing Percona MySQL

Once this extension is installed either as standalone or as part of an
extension set we can then install mysql.

    sm percona install

Then continue using the 'sm mysql' extension for all other operations, see the
README of that extension.

