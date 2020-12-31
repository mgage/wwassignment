# wwassignment

 Active development of this Moodle module has moved to this site: wwassignment on https://github.com/openwebwork from it's original host at github.com/mgage

1. August 28, 2017: The merged pull request ver3.1 updates wwassignment to work with moodle 3.*
Read the comments on https://github.com/openwebwork/wwassignment/pull/3 for more detail.  The pull requests
changes how wwassignment determines whether there has been recent assignment activity when performing the grade 
update cron job.  The change was required to conform to the new way in which activities are logged in moodle 3.* vs moodle 2.8
2. Sept 5, 2019: This still works with Moodle 3.3.4 (for example https://demo.webwork.rochester.edu/moodle) but the wwassignment module may require further updates to work with Moodle 3.5 and later. 
3. Connecting WeBWorK to Moodle using LTI is also possible (follow the same directions as connecting WeBWorK to Canvas, Blackboard, D2L and so forth. LTI has the automatic single sign-on capabilities of wwassignment but LTI-1.2 does not have the bandwidth to transmit all homework information back to the gradebook. 

http://webwork.maa.org/wiki/LTI-Advanced_Authentication

http://webwork.maa.org/wiki/LTI-Advanced_Grading (limited grade passback)


## Moodle WeBWorK assignment activity module

**wwassignment** and **wwlink** provide a reliable method of presenting introductory and 
advanced mathematics assignments through the Moodle LMS.  

This repository contains a branch that works with Moodle 1.9.8, the last of the Moodle 1.x versions, 
as well as a branch that works with  Moodle 2.8.x versions including at this writing version 2.8.5.
The wwassignment branch ver3.0 and the wwlink branch ver 2.8 are compatible with Moodle 3.x (so far).   

The original version of this software "wwmoodle" was written by Peter Snoblin at Truman State University
in 2005 to connect WeBWorK1 and Moodle 1.  Additional development during 2006 and 2007 
by Michael Gage and then by Matt Leventi at the University of Rochester 
produced a robust connection between evolving versions of Moodle1 and WeBWorK2. 

Jonathan Duncan at Walla Walla University made modifications which allowed 
these modules to continue to work with Moodle 2.0.
(This is essentially the ver2.6+ branch of this repository.) 

Most recently (2014-2015) Michael Gage with help from  Nelson Moller (Cégep à Distance) have overhauled the 
modules, removing spurious error messages, modifying the backup code and 
making adjustments so that these modules now work well with the latest version of Moodle 2.8.5.
The original "wwmoodle" repository has been split into "wwassignment" and "wwlink" so 
that they are easier to install.

Quick install **wwlink**:

1. cd moodle/blocks
2. git clone https://github.com/openwebwork/wwlink.git

Quick install **wwassignment**:

1. cd moodle/mod
2. git clone https://github.com/openwebwork/wwassignment.git

For most installations you will want to use the default branch which is ver2.8+

A moodle administrator will need to log in to Moodle from the web in order to activate the two modules and 
to configure the wwassignment preferences so that it points to a local webwork server. 

For more details see the file "INSTALL and CONFIGURE" which also 
describes how to enable the WeBWorK webservice at the WeBWorK installation.

Finally there is much expertise and support for using Moodle and WeBWorK together on the 
forum.

http://webwork.maa.org/moodle/mod/forum/index.php?id=3
