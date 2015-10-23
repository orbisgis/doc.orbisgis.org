Main Components 
========

Here is a list of the main components of OrbisGIS. Except for the map, these components can be: 

- made visible or not *(just close the component to hide it)*,
- resized *(using the cursor of your mouse)*, 
- moved *(drag & drop the component to a new place in the UI)*,
- (un)docked *(pretty useful if you have a dual screen)*.


.. image:: ../_images/orbisgis_main_components.png
              :alt: OrbisGIS main components

To load a component, check the list in the "Windows" menu *(in red in the illustration above)*.


Geocatalog
---------------

The Geocatalog is the place where datasources are managed. Through a right-click in the blank area, the user can:

- Add a datasource *(a file or a folder)*,
- Import a datasource *(a file or a folder)*,
- Remove a datasource,
- Clear the Geocatalog : all the sources are removed from OrbisGIS,
- Show the attributes tables,
- Export layers into flat files or databases.

Map
---------------

The map is the place where geographic informations (vector or raster) are displayed. The user can navigate into the map (using zoom or pan tools), select and get informations on objects.


TOC
---------------

TOC stands for "Table Of Content". This component allows the user to:

- Make visible or not the layer with the checkbox (on the left),
- Change the layer name --> make a double-click on the layer. Then change the name and press “Entrer”,
- Change the order of layers --> drag & drop the layer upward or downward.

Moreover, several features are available via a right-click:

- Edit legend : To change the appearance of the layer or to make a thematic analysis,
- Zoom to layer : Extended zoom on the layer,
- Export : Save the layer in a file *(e.g : into a shape file)* or into a database,
- Remove layer : Remove the layer from the TOC,
- Show attributes : show the attributes's table,
- Start edition : To edit a layer *(e.g: add a field, delete an object, …)*.


DB Tree
---------------

The DB Tree is a tree representation of all the layers loaded in OrbisGIS. Layers (tables) are listed into their respectives folder (views).
Specific options allows the user to:

- Create (spatial) index,
- Remove columns.

Output console
---------------

The output console is the place where all messages (informations, warnings or errors) are displayed.

SQL console
---------------

The SQL console is the place where the user can execute SQL scripts. This component can be considered as a text editor. The user is able to:

- Load & Save .sql files,
- Write instructions,
- Search (spatial) SQL functions and operators into a predetermined list,
- Search & Replace words *(with advanced options)*,
- Share SQL instructions via email *(need a specific plugin)*,
- To auto-complete instructions *(see more below)*.

**Auto-completion**

To use the auto-completion, just press "Ctrl + Space". For example, if you write “sel” and then press “Ctrl + Space”, OrbisGIS will recognize that you want to write “SELECT”. In the same spirit, if you start writing the name of a function, a table or field, a dropdown list will appear on the right to offer you the corresponding elements.

See an illustration video_.

.. _video: https://www.youtube.com/watch?v=neFpyo2qaAI

N.B: This component is available through the "Tools" menu.