
STEP 1:
========
install vault by download from adobe aem cloud

https://www.adobeaemcloud.com/content/companies/public/adobe/filevault/filevault.html

or else it has in /opt directly just unzip it.

unzip C:\AEM New Server\crx-quickstart\opt\filevault\filevalut.zip which is default there.

C:\AEM\crx-quickstart\opt\filevault\filevault\vault-cli-3.1.6\bin.


STEP 2:
=======

Add C:\AEM New Server\crx-quickstart\opt\filevault\vault-cli-3.1.6\bin to path system environment variable. to run
from command prompt.

STEP 3:
=======
Checking out the repository 

command:
========
    
    c:\Arun> svn co http://svn.server.com/repos/myproject
    
STEP 4:
=======

Synchronizing with the repository
==================================

You need to synchronize filevault with the repository. To do this:
In the command line, navigate to content/jcr_root.
Check out the repository by typing the following (substituting your port number for 4502 and your admin passwords):
       	
    c:\Arun> vlt --credentials admin:admin co --force http://localhost:4502/crx
   
   

