
RPM build instructions:  3 options
==================================

Prerequisites
-------------

Ensure that you have a .rpmmacros file in your $HOME directory.
A sample of this file is provided in rpmmacros.sample.

Option 1: Regular build
-----------------------

Run 'mvn clean install'.  This will download and build the source, and create the RPM.

Option 2: Build manually from SVN
---------------------------------

1) mkdir jboss-eap-5.0-src; cd jboss-eap-5.0-src
2) svn co http://anonsvn.jboss.org/repos/jbossas/tags/JBPAPP_5_0_0_GA jboss-as
3) cd jboss-as/build
4) ant
5) cd ../../..
6) mvn clean install -Djboss.skip.download -Djboss.skip.unzip -Djboss.skip.build

Option 3: Download the binary
-----------------------------

1) Download the binary (login required) [1]
2) mkdir -p jboss-eap-5.0-src/jboss-as/build/output/jboss-5.0.0.GA
3) unzip <zipfile> -d jboss-eap-5.0-src/jboss-as/build/output/jboss-5.0.0.GA
4) mvn clean install -Djboss.skip.download -Djboss.skip.unzip -Djboss.skip.build  

Successful build: The RPM
-------------------------

The resulting RPM is located in target/rpm/jboss-eap/RPMS/

[1] https://support.redhat.com/jbossnetwork/restricted/listSoftware.html?product=appplatform

