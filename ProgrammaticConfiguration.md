# Introduction #

The first time that a user navigates to the application, the program will walk the user through entering various configuration settings such the database settings and authentication settings. These settings, for now, will be stored in a Properties file which will be checked for by the Bootstrap servlet. If the Bootstrap servlet successfully loads the configuration Properties on subsequent access to the site, then the user will no longer be asked to configure the application and the information in the Properties file will be used. Perhaps it is also an idea to have an administrator option which allows the Properties file to be deleted and the isConfigured attribute to be reset so that the application can be reconfigured from scratch.

![http://triage.googlecode.com/files/Triage-Config-01.png](http://triage.googlecode.com/files/Triage-Config-01.png)
![http://triage.googlecode.com/files/Triage-Config-02.png](http://triage.googlecode.com/files/Triage-Config-02.png)
![http://triage.googlecode.com/files/Triage-Config-03.png](http://triage.googlecode.com/files/Triage-Config-03.png)
![http://triage.googlecode.com/files/Triage-Config-04.png](http://triage.googlecode.com/files/Triage-Config-04.png)
![http://triage.googlecode.com/files/Triage-Config-05.png](http://triage.googlecode.com/files/Triage-Config-05.png)