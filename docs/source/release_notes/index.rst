Release Notes
=============

Your wait is now over as we are announcing the release 1.8 of Spacewalk, a systems management solution.

The download locations are

* http://yum.spacewalkproject.org/1.8/RHEL/5/$basearch/
* http://yum.spacewalkproject.org/1.8/RHEL/6/$basearch/
* http://yum.spacewalkproject.org/1.8/Fedora/16/x86_64/
* http://yum.spacewalkproject.org/1.8/Fedora/17/x86_64/

with client repositories under

* http://yum.spacewalkproject.org/1.8-client
* http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/1.8/openSUSE_12.1/
* http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/1.8/openSUSE_12.2/
* http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/1.8/openSUSE_Factory/

Features & Enhancements in Spacewalk 1.8
----------------------------------------

* Spacewalk runs on Fedora 17
* Spacewalk can be run on the same machine as Oracle XE 11g
* OpenSCAP functionality extended
* osa-dispatcher is now ``systemd`` service in Fedora
* Server-side support for registering ARM clients
* Integration with SUSE Studio
* Basic ABRT notification
* Distribution-channel mapping can be customized per organization
* Systems requiring reboot view
* Extra packages view
* ``spacewalk-repo-sync`` now downloads comps information, enabling yum group operations
* WebUI and usability improvements
* PostgreSQL improvements
* Cobbler 2.0 now packaged in Spacewalk repos
* Archived actions now can be deleted
* Modified API calls:

  * ``configchannel.createOrUpdatePath`` now accepts also binary attribute and has fixed handling of binary files
  * ``configchannel.lookupFileInfo`` and ``system.getScriptResults`` now returns base64 encoded content for binary files
  * ``system.scap.scheduleXccdfScan`` can be scheduled for multiple servers and with timestamp to fire the scan
  * ``system.provisionVirtualGuest`` accepts MAC address parameter

New API calls:

  * ``channel.software.addRepoFilter``, ``.setRepoFilters``, ```.clearRepoFilters``, ``.removeRepoFilter``, ``.listRepoFilters``
  * ``errata.cloneAsOriginalAsync``, ``errata.cloneAsync``
  * ``kickstart.profile.getCfgPreservation``, ``kickstart.profile.setCfgPreservation``
  * ``schedule.deleteActions``
  * ``system.scap.listXccdfScans``, ``system.scap.getXccdfScanDetails``, ``system.scap.getXccdfScanRuleResults``
  * ``system.listSystemsWithExtraPackages``, ``system.listExtraPackages``, ``system.listActiveSystemsDetails``
  * ``distchannel.listMapsForOrg``, ``distchannel.setMapForOrg``

* We parted with API call:

  * ``distchannel.setDefaultMap``

The up-to-date API documentation can be found at http://www.spacewalkproject.org/documentation/api/

Contributors
------------

Our thanks go to the community members who contributed to this release:

* Aron Parsons
* Duncan Mac-Vicar
* Gael Chamoulaud
* Joerg Steffens
* Johannes Renner
* Jonathan Hoser
* Joshua Roys
* Michael Calmer
* Nigel Jones
* Paresh Mutha
* Pierre Casenove
* Richard Marko
* Stefan Meyer
* Steven Hardy
* Tasos Papaioannou
* Uwe Gansert
* William van de Velde

https://fedorahosted.org/spacewalk/wiki/ContributorList

Some statistics
---------------

In Spacewalk 1.8, we've seen

* 258 bugs fixed
* 1799 changesets committed
* 2506 commits done

User community, reporting issues
--------------------------------

To reach the user community with questions and ideas, please use the `spacewalk-list <https://www.redhat.com/mailman/listinfo/spacewalk-list>`_ mailing list . On this list, you can of course also discuss issues you might find when installing or using Spacewalk, but please do not be surprised if we ask you to file a bug at `<https://bugzilla.redhat.com/enter_bug.cgi?product=Spacewalk>`_ with more details or full logs.

Thank you for using Spacewalk.

Happy birthday, Mirek, Michael, and Stephen.
