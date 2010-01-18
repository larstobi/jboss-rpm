
* Do this before building * 

Download the jboss eap 5.0.0.GA zip file.
unzip the zipfile to src main
E.G: unzip <zipfile> -d src/main/

Ensure that you have a .rpmmacros file in your $HOME directory.
A sample of this file is provided in rpmmacros.sample.

build with 'maven install'.

The RPM file is located here after build: target/rpm/jboss-eap/RPMS/noarch/.