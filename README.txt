
Build instructions
==================

1) Download the jboss eap 5.0.0.GA binary [1] or build it from source [2].

2) unzip the zipfile to src main, e.g.: unzip <zipfile> -d src/main/

3) Ensure that you have a .rpmmacros file in your $HOME directory.
   A sample of this file is provided in rpmmacros.sample.

4) build with 'mvn install'.  The resulting RPM file is 
   located at target/rpm/jboss-eap/RPMS/noarch/.

[1] https://support.redhat.com/jbossnetwork/restricted/listSoftware.html?product=appplatform
[2] http://anonsvn.jboss.org/repos/jbossas/tags/JBPAPP_5_0_0_GA/

