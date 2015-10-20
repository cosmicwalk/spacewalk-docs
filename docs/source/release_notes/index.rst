Release Notes
=============

Your wait is now over as we are announcing the release 1.9 of Spacewalk, a systems management solution.

The download locations are

http://yum.spacewalkproject.org/1.9/RHEL/5/i386/
http://yum.spacewalkproject.org/1.9/RHEL/5/x86_64/
http://yum.spacewalkproject.org/1.9/RHEL/6/i386/
http://yum.spacewalkproject.org/1.9/RHEL/6/x86_64/
http://yum.spacewalkproject.org/1.9/Fedora/17/x86_64/
http://yum.spacewalkproject.org/1.9/Fedora/18/x86_64/

with client repositories under

http://yum.spacewalkproject.org/1.9-client
http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/1.9/openSUSE_12.2/
http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/1.9/openSUSE_12.3/
http://download.opensuse.org/repositories/systemsmanagement:/spacewalk:/1.9/openSUSE_Factory/

Features & Enhancements in Spacewalk 1.9
----------------------------------------

* Spacewalk runs on Fedora 18
* ABRT enhancements/improvements to make more functional

  * https://fedorahosted.org/spacewalk/wiki/HowToUseCrashReporting

* SCAP improvements

  * Support for XCCDF 1.2
  * Allow ``--cpe`` command-line argument to oscap

* WebUI Login extended for expired Spacewalk Certificates, from 7 days to 30 days [Satellite driven]
* WebUI Enhancements

  * Display Activation key used to register, on system profile page
  * Highlightning of hovered row in tables
  * CSS rules for printing of WebUI pages
  * Link associated errata to package from package overview page
  * Added CVS download/report of Software Channel Entitlements

* Bug 877451 - yum-like per-repo configuration for ``spacewalk-repo-sync``
* ``rhnmd`` works with Fedora systemd Service for startup
* Move to newer tomcat for Fedora based Spacewalk
* Bug 878216 - make ``rhncfg`` diff output configurable
* Updates to ``spacewalk-repo-sync``:

  * Syncing over SSL and IPv6 works correctly
  * Sync Kickstart Trees (Distributions)

* New features related to Kickstarting systems:

  * Allow the selection of a primary network interface from hardware profile
  * Allow Kickstart Profile to automatically update to newest applicable Distribution

* New reports added to spacewalk-reports:

  * ``custom-info``
  * ``inactive-systems``
  * ``inventory (modified)``
  * ``packages-updates-all``
  * ``packages-updates-newest``
  * ``system-currency``
  * ``system-groups``
  * ``system-groups-keys``
  * ``system-groups-systems``
  * ``system-groups-users``
  * ``system-packages-installed``

* Modified API calls:

  * ``channel.software.clone``
  * ``org.delete``
  * ``kickstart.profile.setAdvancedOptions``
  * ``errata.setDetails``
  * ``errata.findByCve``

* New API calls:

  * Everything under system.crash, including:

    * ``system.crash.deleteCrash``
    * ``system.crash.getCrashFile``
    * ``system.crash.getCrashFileUrl``
    * ``system.crash.getLastReportDate``
    * ``system.crash.getTotalCrashCount``
    * ``system.crash.getUniqueCrashCount``
    * ``system.crash.listSystemCrashFiles``
    * ``system.crash.listSystemCrashes``

  * ``kickstart.importFile (variant)``
  * ``kickstart.createProfile (variant)``
  * ``kickstart.createProfileWithCustomUrl (variant)``
  * ``kickstart.importRawFile (variant)``
  * ``kickstart.profile.getUpdateType``
  * ``kickstart.profile.setUpdateType``
  * ``system.deleteSystem (variant)``
  * ``system.listAllInstallablePackages``
  * ``system.setPrimaryInterface``
  * ``org.getCrashFileSizeLimit``
  * ``org.setCrashFileSizeLimit``

The up-to-date API documentation can be found at http://www.spacewalkproject.org/documentation/api/

Contributors
------------

Our thanks go to the community members who contributed to this release:

* Aron Parsons
* David Juran
* Duncan Mac-Vicar
* Joerg Steffens
* Johannes Renner
* Jose Simonelli
* Marcelo Moreira de Mello
* Mark Huth
* Michael Calmer
* Neha Rawat
* Nigel Jones
* Paresh Mutha
* Pierre Casenove
* Zailo Leite

https://fedorahosted.org/spacewalk/wiki/ContributorList

Some statistics
---------------

In Spacewalk 1.9, we've seen

* 86 bugs fixed
* 676 changesets committed
* 1055 commits done

User community, reporting issues
--------------------------------

To reach the user community with questions and ideas, please use the `spacewalk-list <https://www.redhat.com/mailman/listinfo/spacewalk-list>`_ mailing list . On this list, you can of course also discuss issues you might find when installing or using Spacewalk, but please do not be surprised if we ask you to file a bug at `<https://bugzilla.redhat.com/enter_bug.cgi?product=Spacewalk>`_ with more details or full logs.

Thank you for using Spacewalk.
