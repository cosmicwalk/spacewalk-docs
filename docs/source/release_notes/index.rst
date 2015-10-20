Release Notes
=============

Hello everyone,

We are proudly announcing release of Spacewalk 2.4, a systems management solution.

The download locations are

* http://yum.spacewalkproject.org/2.4/RHEL/6/
* http://yum.spacewalkproject.org/2.4/RHEL/7/
* http://yum.spacewalkproject.org/2.4/Fedora/21/
* http://yum.spacewalkproject.org/2.4/Fedora/22/

with client repositories under

* http://yum.spacewalkproject.org/2.4-client/RHEL/5/
* http://yum.spacewalkproject.org/2.4-client/RHEL/6/
* http://yum.spacewalkproject.org/2.4-client/RHEL/7/
* http://yum.spacewalkproject.org/2.4-client/Fedora/21/
* http://yum.spacewalkproject.org/2.4-client/Fedora/22/

SUSE Linux client packages can be found here

* http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/2.4/openSUSE_13.1/
* http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/2.4/openSUSE_13.2/
* http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/2.4/openSUSE_Tumbleweed/
* http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/2.4/SLE_12/
* http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/2.4/SLE_11_SP4/

For fresh installations, please use steps from

* :ref:`installation-guide`

If you plan to upgrade from older release, search no more -- the following page will guide you:

* :ref:`upgrade-guide`

Features & Enhancements in Spacewalk 2.4
----------------------------------------

* Spacewalk now supported on Fedora 22
* Spacewalk supports Fedora 22 clients

  * New package - ``dnf-plugin-spacewalk``

* Organization-specific configuration moved to Organization Admin menu

  * Satellite admins can allow/disallow Organization admins to manage this configuration

* Passwords are not sent to user in clear text anymore

  * https://fedorahosted.org/spacewalk/wiki/Features/ResetPassword

* Continued UI polish and improvements, including standardizing on `Patternfly <https://www.patternfly.org/>`_
* Plenty of small enhancements and fixes

  * Added support for Catalan and Portuguese translations from Zanata project
  * Fedora and RHEL/CentOS 7 Cobbler provisioning fixes
  * Removed checksum type None for software channels
  * Fixed system.listUngroupedSystems API call
  * Repository sync page improved to show more details about last sync
  * Repository sync option for syncing latest packages only added
  * Osa ping API calls added
  * Added compliancy indicator icon on Scap results list page

* New API calls:

  * ``org.isErrataEmailNotifsForOrg``
  * ``org.isOrgConfigManagedByOrgAdmin``
  * ``org.setErrataEmailNotifsForOrg``
  * ``org.setOrgConfigManagedByOrgAdmin``
  * ``system.getOsaPing``
  * ``system.sendOsaPing``

The up-to-date API documentation can be found at http://www.spacewalkproject.org/documentation/api/2.4/

Contributors
------------

Our thanks go to the community members who contributed to this release:

* Amar Huchchanavar
* Anastasios Papaioannou
* Aron Parsons
* Avi Miller
* David Holland
* David Hrbáč
* Duncan Mac-Vicar P
* Frantisek Kobzik
* Hubert Mantel
* Jared Greenwald
* Johannes Renner
* Kevin Walter
* Klaas-
* Marcelo Moreira de Mello
* Martin Seidl
* Matej Kollar
* Michael Calmer
* Michael Kromer
* Michael Mattioli
* Michael Mraka
* Miroslav Suchý
* Patrick Hurrelmann
* Paul Wayper
* Pavel Studenik
* Shannon Hughes
* Silvio Moioli
* Stephen Herr
* Šimon Lukašík
* Tasos Papaioannou
I Thomas Mueller

https://fedorahosted.org/spacewalk/wiki/ContributorList

Some statistics
---------------

In Spacewalk 2.4, we've seen

* 59 bugs fixed
* 428 changesets committed
* 705 commits done

Github repo for commits since Spacewalk 2.3

* `Spacewalk 2.3 to 2.4 <https://github.com/spacewalkproject/spacewalk/graphs/contributors?from=2015-03-27&to=2015-09-29&type=c>`_

User community, reporting issues
--------------------------------

To reach the user community with questions and ideas, please use `spacewalk-list <https://www.redhat.com/mailman/listinfo/spacewalk-list>`_ mailing list. On this list, you can of course also discuss issues you might find when installing or using Spacewalk, but please do not be surprised if we ask you to `file a bug <https://bugzilla.redhat.com/enter_bug.cgi?product=Spacewalk>`_ with more details or full logs.

Thank you for using Spacewalk.


