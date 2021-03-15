# Pentaho-Kettle---installation
Kettle is an opensource, comprehensive alternative for traditional data integeration tools like Informatica PowerCenter, IBM InfoSphere DataStorage, BusinessObjects Data Integrator and SAS Data Integration Studio. Purpose of this repository is to provide an instruction for installation.
(END RESULT (see files) = .OVA file (file used to describe the virtual machine, can be imported in VirtualBox))
### Prerequisites
#### 1) Create a Virtualbox image with your preferred Operating System (Linux AntiX)
I choose Linux Antix. Reason: Very small on resource 500MB memory, 4G storage. Free. Debian-based (=lots of software repositories available).
<br>
<code>antiX - antiX-19.3_386-full.iso. (Might be better to use 64-bits version, I went for small)
VirtualBox - New - Choose VDI - 8GB minimum, 500MB memory, ISO -> antiX-19.3...
Install antiX on new machine.
</code>
<br>
#### 2) Install java 8
(https://stackoverflow.com/questions/55920389/e-package-oracle-java8-installer-has-no-installation-candidate)
##### Add the following line to /etc/apt/sources.list:
<code>deb https://debian.opennms.org/ stable main</code>
##### Install GPG key of the repository:
<code>wget -O - http://debian.opennms.org/OPENNMS-GPG-KEY | sudo apt-key add -</code></code>
##### Update the package index:
<code>sudo apt-get update</code>
##### Install oracle-java8-installer deb package:
<code>sudo apt-get install oracle-java8-installer</code>

#### 3) Install libjavascriptcoregtk-1.0-0
(https://debian.pkgs.org/9/debian-main-i386/libjavascriptcoregtk-1.0-0_2.4.11-3_i386.deb.html)
##### get libwebkitgtk-1.0-0_2.4.11-3_i386.deb:
<code>apt install ./libwebkitgtk-1.0-0_2.4.11-3_i386.deb</code>
##### get libicu57-1.0-0_2.4.11-3_i386.deb:
<code>apt install ./libicu57-1.0-0_2.4.11-3_i386.deb</code>
##### get libjavascriptcoregtk-1.0-0.deb:
<code>apt install ./libjavascriptcoregtk-1.0-0.deb</code>
