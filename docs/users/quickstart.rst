Quickstart 
==========


The workspace
---------------

The workspace is the configuration of your User Interface *(UI)*.

The following items are saved in the workspace:

- opened windows (with their size and place in the UI),
- database connection parameters,
- map context file (loaded layers in the TOC),
- toolbox parameters


Database
---------------

OrbisGIS is build on top of a relational spatial database. All data are managed, queried from a JDBC driver.
By default OrbisGIS starts with the embedded spatial database H2GIS. However, OrbisGIS could be connected to a PostgresSQL-PostGIS database.



Load data
---------------

To load data, just choose "Add" or "Import" in the Geocatalog.

Note : because of OrbisGIS uses a RDBMS, a data is represented as a table and could be requested using the SQL languague.


Display on the map
------------------

To display a geographic layer, just drag & drop it from the Geocatalog to the TOC.


Display attributes
------------------

To see how to display attributes, have a look at :ref:`show_attributes` page.

