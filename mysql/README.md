# SM Framework MySQL Extension

## Prerequisites
First ensure that gcc version 4.2.1 or later is installed.

Next ensure that readline along with it's development headers are installed.
On an rpm based system this is typically done with:

    yum install -y readline readline-devel


The cmake tool is required before being able to install mysql (in
addition to the standard gcc tool chain) You can install cmake using the
SM Framework tools extension set as follows:

    sm set install tools
    sm cmake install

## Installing MySQL

Once this extension is installed either as standalone or as part of an
extension set we can then install mysql.

    sm mysql install

## Initializing the database

Once mysql has been installed you must then initialize the actual database
directory which is done by:

    sm mysql initialize

## Configuring mysql

Next we configure mysql including (as root) linking the /etc/mysql/mysql.cnf

    sm mysql configure

## Controlling mysql

In order to control the mysql server we run the following commands:

    sm mysql start
    sm mysql stop
    sm mysql restart

