
			   Welcome to Rudix, Comrade!

   Rudix for power users is a world class collection of pre-compiled and ready to use Unix compatible software (packages) which are not available from a standard installation of Mac OS X (or Darwin) and is very popular among Unixes environments like GNU/Linux and FreeBSD. For example, software like wget, ncftp, lynx and many more command line tools.

   Rudix for system administrators and developers is a powerful and easy to customize mechanism to retrieve, compile and create native Mac OS X packages (.pkg files). Rudix is very similar in concept to BSD's ports system and is proud to keep this tradition of simplicity and elegance.
   I'm A Power User. How Do I Install Rudix?

   Before you can install and use any package you have to add two paths to your $PATH variable environment. You can do it locally (for one user) or globally (for everybody).

   For one user add the following lines to your $HOME/.profile (or .bash_profile) file to

   PATH="$PATH:/usr/local/bin:/usr/local/sbin"
   export PATH

   For system wide usage change your /etc/profile file to

   PATH="/bin:/sbin:/usr/bin:/usr/sbin:/usr/local/bin:/usr/local/sbin"
   export PATH

   now you are ready to install packages provided by Rudix.

   Packages:

   Name Version Description
   [1]ccache 2.4 Acts as a caching pre-processor to C or C++ compilers
   [2]dictd 1.9.15 Dict is a client for the Dictionary Server Protocol (DICT)
   [3]gnupg 1.4.2 GnuPG is a complete and free replacement for PGP
   [4]inadyn 1.96 Simple DYNAMIC DNS client
   [5]lynx 2.8.5 Lynx is a fully-featured World Wide Web (WWW) text mode client
   [6]ncftp 3.1.9 NcFTP is a free set of programs that use the File Transfer Protocol
   [7]p7zip 4.20 p7zip is a quick port of 7z.exe and 7za.exe for Unix. 7-Zip is a file archiver with highest compression ratio
   [8]subversion 1.2.3 The goal of the Subversion project is to build a version control system that is a compelling replacement for CVS
   [9]nmap 3.93 Nmap is a free open source utility for network exploration or security auditing
   [10]wget 1.10.1 GNU Wget is a free utility for non-interactive download of files from the Web

   All those packages were compiled and tested on Mac OS X 10.3 (Panther).  I bet those packages works on Mac OS X 10.4 (Tiger) too, feedbacks are welcomed!

   I'm A System Administrator Or Developer. How Do I Install Rudix?

   For system administrators and developers interested in Rudix as a port system I recommend to use the CVS to retrieve Rudix, see the [11]CVS repository but basically you do:

   $ CVSROOT=:pserver:anonymous@cvs.sourceforge.net:/cvsroot/rudix
   $ cvs login
   (Logging in to anonymous@cvs.sourceforge.net)
   CVS password:  press return
   $ cvs -z3 co rudix
   U rudix/COPYING.txt
   U rudix/README.txt
   ...
   $ cd rudix/ports/ccache
   $ make pkg

   to build and create a package of ccache in the current port directory.

   Note that [12]DeveloperTools is required in order to use the port system because we need the GCC compiler kit and some libraries and tools which DeveloperTools provides to build any software.

   FAQ
   Q. Why Rudix install packages in /usr/local?
   A. Because it is the standard place for third party software.
   Q. How do I uninstall a package?
   A. Mac OS X does not provides any graphical uninstaller, but you can uninstall Rudix's packages by running /usr/local/sbin/uninstall-package.sh script. You must run it as root or prefix the script with sudo to work.
   Q. I didn't like Rudix. Is there any alternative?
   A. Yes, take a look at [13]DarwinPorts or [14]Fink.
   Q. What are the advantages of Rudix against the others?
   A. Simplicity. All packages are self-contained and installable via disk image, you don't need to use any other package management tool to install those softwares.
   Q. What does Rudix means? Is it a combination of your name and Unix or what?
   A. Rudix stands for "Unix for Commies" but in fact I'm not communist ;) it's a joke.

   Other Resources
     * [15]Project information on SourceForge
     * [16]Project details on Freshmeat
     * [17]Rudix News
     * [18]Full package list with MD5 checksum

   Copyright and License

   Rudix is copyrighted by Rudá Moura and is licensed under [19]GPL. The Rudix logo is provided by Elvis Pfützenreuter. Thank you right winger comrade!

   © 2005 Rudá Moura

   [20]SourceForge.net Logo 

References

   1. http://prdownloads.sourceforge.net/rudix/ccache-2.4.dmg?download
   2. http://prdownloads.sourceforge.net/rudix/dictd-1.9.15.dmg?download
   3. http://prdownloads.sourceforge.net/rudix/gnupg-1.4.2.dmg?download
   4. http://prdownloads.sourceforge.net/rudix/inadyn-1.96.dmg?download
   5. http://prdownloads.sourceforge.net/rudix/lynx-2.8.5.dmg?download
   6. http://prdownloads.sourceforge.net/rudix/ncftp-3.1.9.dmg?download
   7. http://prdownloads.sourceforge.net/rudix/p7zip-4.20.dmg?download
   8. http://prdownloads.sourceforge.net/rudix/subversion-1.2.3.dmg?download
   9. http://prdownloads.sourceforge.net/rudix/nmap-3.93.dmg?download
  10. http://prdownloads.sourceforge.net/rudix/wget-1.10.1.dmg?download
  11. http://sourceforge.net/cvs/?group_id=146701
  12. http://www.apple.com/macosx/developertools/
  13. http://darwinports.opendarwin.org/
  14. http://fink.sourceforge.net/
  15. http://sourceforge.net/projects/rudix
  16. http://freshmeat.net/projects/rudix/
  17. http://sourceforge.net/news/?group_id=146701
  18. http://sourceforge.net/project/showfiles.php?group_id=146701
  19. http://www.gnu.org/copyleft/gpl.html
  20. http://sourceforge.net/
