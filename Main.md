# Introduction #

> When I started this project, I was looking for a help desk application which would leverage previous work to make solving common problems quick and simple. The idea is that as a technician enters a new ticket, the application will present them with previous tickets/solutions which may be related and be able to present a quick answer. This way, knowledge is not lost and can be easily leveraged even with new personnel in the IT work force.

# Philosophy #

> The application should be designed to be extensible in several ways. One method is the authentication subsystem. The initial release should support Active Directory, LDAP, and SQL based authentication. Each of these should implement the "AuthProvider" interface as a way to make the authentication classes compatible.

> Another area which should be extensible is the methods by which tickets can be created. For my environment, I intend to implement ticket generators for our OpenNMS system and allow our Asterisk IP PBX to create a ticket when our Help Desk phone line is answered. Other plug-ins could conceivably be produced to integrate with Nagios, Tivoli, OpenView, etc....

> Finally, I would like to the application to be a Rich Internet Application through the use of the [ZK](http://www.zkoss.org/) framework.

# Status #

> I have hardly even begun. So far I have an initial design for the data structure via Hibernate annotations. The initial configuration interface is coming along nicely. The initial data structures still need to be expanded to handle asset tracking and project management. A mock-up of the user interface has been started, but it is only for design testing purposes.

> I have also started modifying the code to be as modular as possible. The authentication providers are now self-contained (including configuration interfaces) and the first generator for IMAP is also self-contained with configuration interface as well. This means that down the road, it should be possible to make new generators and auth providers drop in compatible with the application.