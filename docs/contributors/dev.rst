.. Author : Gwendall PETIT (Lab-STICC - CNRS UMR 6285 / DECIDE Team)

Develop 
========


Source code
-----------------------

OrbisGIS is a free and open-source GIS software, released under the `GPL v3`_ licence. You can access to the source code on the dedicated GitHub_ repository.

.. _GitHub: https://github.com/orbisgis/orbisgis/

Developers are cordially invited to contribute to OrbisGIS, posting:

* Issues: detect a bug, ask for enhancement ? `Create an issue`_ on GitHub,
* `Pull Request`_ (PR): want to contribute ? Please submit your PR and we will analyze it carefully.

.. _Create an issue: https://github.com/orbisgis/orbisgis/issues/new
.. _Pull Request: https://github.com/orbisgis/orbisgis/pulls


Tools for developers
----------------------------

The following two "Continuous Integration" tools are used to build, control and deploy OrbisGIS source code:

* `Jenkins server`_
* `Travis`_

.. _Jenkins server: http://jenkins.orbisgis.org/
.. _Travis: https://travis-ci.org/orbisgis/orbisgis

Releases & Snapshot
----------------------------

* Releases and pre-releases versions can be found `HERE`_
* Daily snapshot release *(for test purpose)* is provided via:
	* a `.zip`_ file *(works on Linux, Windows and macOS)*,
	* a `.deb`_ file *(for amd64 architecture / also available for* `i386`_ *)*,
	* the :ref:`Ubuntu_PPA_repository`.

.. _HERE: https://github.com/orbisgis/orbisgis/releases
.. _.zip: http://jenkins.orbisgis.org/job/orbisgis/lastSuccessfulBuild/artifact/orbisgis-dist/target/orbisgis-bin.zip
.. _.deb: https://launchpad.net/~orbisgis/+archive/ubuntu/orbisgis-unstable/+files/orbisgis_5.1.0-snapshot513-1_amd64.deb 
.. _i386: https://launchpad.net/~orbisgis/+archive/ubuntu/orbisgis-unstable/+files/orbisgis_5.1.0-snapshot513-1_i386.deb

Wiki documentation
--------------------------

Below are some useful links for developers, that are mainly provided on the wiki_ page of the OrbisGIS GitHub repository.

.. _wiki: https://github.com/orbisgis/orbisgis/wiki


* `How to build OrbisGIS ?`_
* `Debugging OrbisGIS with maven`_
* `OrbisGIS and Nexus`_
* `Release on Maven Central`_
* `OrbisGIS internals`_
* `OrbisGIS plugin system`_
	* `Create your plugin`_
	* `Resolve your plugin's dependencies`_


.. _How to build OrbisGIS ?: https://github.com/orbisgis/orbisgis/wiki/2.-Building-OrbisGIS
.. _Debugging OrbisGIS with maven: https://github.com/orbisgis/orbisgis/wiki/3.-Debugging-OrbisGIS-with-maven
.. _OrbisGIS and Nexus: https://github.com/orbisgis/orbisgis/wiki/4.-OrbisGIS-and-Nexus
.. _Release on Maven Central: https://github.com/orbisgis/orbisgis/wiki/5.-Release-on-Maven-Central
.. _OrbisGIS internals: https://github.com/orbisgis/orbisgis/wiki/7.-OrbisGIS-internals
.. _OrbisGIS plugin system: https://github.com/orbisgis/orbisgis/wiki/8.-OrbisGIS-plugin-system
.. _Create your plugin: https://github.com/orbisgis/orbisgis/wiki/8.1.-Create-your-plugin
.. _Resolve your plugin's dependencies: https://github.com/orbisgis/orbisgis/wiki/8.2.-Resolve-your-plugin's-dependencies
 


Additional informations
-----------------------------

* Made by a `team`_ from `CNRS`_
* Registered date : 22/12/2007
* Langage of development : 100% Java
* Licence : `GPL v3`_
* Supported OS : Linux, Windows and Mac OS
* Installation requirement : at least Java 7

.. _team: https://github.com/orbisgis/orbisgis/wiki/1.-Team
.. _CNRS: http://www.cnrs.fr/
.. _GPL v3: https://www.gnu.org/licenses/quick-guide-gplv3.en.html


