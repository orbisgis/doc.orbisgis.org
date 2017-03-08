.. Author : Gwendall PETIT (Lab-STICC - CNRS UMR 6285 / DECIDE Team)

Groovy script with SQL 
======================

Below is an example of how to use SQL instructions into Groovy script.

.. code-block:: groovy
   
	import groovy.sql.Sql;

	def sql = Sql.newInstance(grv_ds);

	// Execute SQL request
	sql.execute("DROP TABLE IF EXISTS TEST")
	sql.execute("CREATE TABLE TEST AS SELECT 'POINT(1 3 10)'::geometry THE_GEOM")

	// Fetch results and print point coordinates
	// row["THE_GEOM"] is an instance of 
	// http://tsusiatsoftware.net/jts/javadoc/com/vividsolutions/jts/geom/Point.html
	sql.eachRow("SELECT * FROM TEST") { row ->
	    pt = row["THE_GEOM"].getCoordinate()
	    print(pt.x+" "+pt.y+" "+pt.z)
	}



To see more, you can consult this tutorial_ from the Groovy documentation.


.. _tutorial: http://docs.groovy-lang.org/latest/html/documentation/#_interacting_with_a_sql_database
