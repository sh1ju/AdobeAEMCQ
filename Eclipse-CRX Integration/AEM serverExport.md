in Eclipse you can see AEM server , you could see AEM server only to
the project which is connected to crx.

NOTE:
====
if you give the below command only ui.apps is connect /sync to crx. hence when for instance
you create a NEW SERVER  > Adode > Adobe Experience Manager> when selecting the Maven module projects
you can see now ui.apps and core will be displayed. because project with pom.xml packaging type
pom, or content_type will be displayed . packaging bundle type wont be shown.  

    G:\AEM\webapi\ui.apps\src\main\content\jcr_root>vlt --credentials admi n:admin co --force http://localhost:4502/crx



NOTE:
=====
if you close any project like dependencies it won't show up when try to add modules to server or when doing
create new server > add modules it shows " There are no resources that can be added or removed from server"
when adding or editing or deleting any sub-modules in root also will get reflected in outside view.
for e.g any change in -webapi>core>pom.xml will get reflected in external view created outside core>pon.xml.
so you can work module inside root itself to avoid confusion.

    -dependencies
    -core
    -ui.apps 
    -webapi 
         -core
         -ui.apps
         -dependencies.



1)usually pom.xml bundle packaging wont show in server.

you can change bundle settings:

double on aem server instance >

install > install bundles directly from the filesystem.

you can also check on install bundles via bundle upload.