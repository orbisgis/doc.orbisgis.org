.. Author : Gwendall PETIT (Lab-STICC - CNRS UMR 6285 / DECIDE Team)

Translate 
============

The translation of OrbisGIS is managed thanks to the Transifex_ platform, a free-to-use website enabling users to collaboratively translate open-source projects. To do so, you just have to create a free account. Then, you can access to the Transifex OrbisGIS project HERE_.


.. _Transifex: http://www.transifex.com/
.. _HERE: http://www.transifex.com/projects/p/orbisgis/


.. image:: ../_images/translation.png
              :alt: Translation
              :align: center


Team
---------------------

A langage is manage by a team, which is composed of 3 rules:

* coordinator: manage the team (add/remove members),
* revisor: can translate and validate the result,
* translator: can translate.

*Remark: note that one user can have the 3 rules in the same time.*

New users are invited to:

* create a new team if their langage is not already present,
* or to join an existing team.


Getting started (for translators)
----------------------------------------

Once you are team member, you should be allowed to translate the application. Here you are asked to translate words (also nammed keys) presents in .xml files called *ressources*.


Most of the translation keys are single words or sentences. In this case, the translation process is self-explanatory.
However, you can discover some specific characters such as {} or &. In this case, please follow the instructions below.

1- Curly braces
*****************************


In some cases, you will notice a number enclosed by curly braces. These strings refer to special parameters in the code and must be preserved. For example, the French translation of {0}_selection_{1} is {0}_sélection_{1}. Here {0} refers to the layer name and {1} refers to a text value.

Another example:

.. code-block:: bash

    Cannot add a LayerCollection {0}.

becomes in French

.. code-block:: bash

    Impossible d'ajouter la collection de couche {0}.


2- & symbol
*****************************

The & symbol is used to create keyboard shortcuts. So they have to be preserved (if possible).

Example:

.. code-block:: bash

    &Copy

becomes in French

.. code-block:: bash

    &Copier

In this example, the shortcut will be placed on the “C”.


Contributors
----------------------------------------

Contributions are welcome! You can help out by translating, proofreading existing translations, or creating your own translation team (for a new language).

If your translation looks good, your work will be integrated into OrbisGIS.

Already done:

* English,
* French.

Languages in progress:

* Italian: Thanks to Simone Sandri (aka xseris), Team manager
* Portuguese (Brazil): Thanks to Enrico Nicoletto, Team manager,
* Arabic: Thanks to Ilyes Smadi (aka Smadi), Team manager,
* Chinese: Thanks to Quing-Xia Zhou, Team manager, Yinghao Li and Su Qi
* Spanish: Thanks to Emilio Plaza García (aka Dharth),
* Persian: Thanks to Mohammad Hosseini (aka PersianPolaris), Team manager and Mehrazin Omrani (aka Azin),
* Russian: Thanks to Assem, Team manager,
* Greek: Thanks to Ioannis Tsimpiris (aka gtsimp), Team manager,
* Breton


Transifex configuration (for developers)
-------------------------------------------------

The python file in tools will call `mvn gettext:gettext` in order to update all .pot files in the project tree.

To send to transifex new translation keys:

.. code-block:: bash

	cd tools/
	python internat.py
	tx push -s


To retrieve updated translations from transifex.

.. code-block:: bash

	tx pull -a --minimum-perc=1


This will update all .po files. A commit then a pull request has to be done in order to be published into the final binary.


