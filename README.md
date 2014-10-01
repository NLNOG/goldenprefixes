Introduction
------------

This files are part of the Hijack Mitigation Project (hmproject), as introduced
by Jared Mauch at NANOG62.

discussion mailinglist: hmproject@puck.nether.net 

(recommendations for additions allowed after being vouched for by two people)

Directory Layout
----------------

Each Autonomous System is represented by a directory starting with 'AS'
followed by the number. In each of these AS specific directories two files
are present: 'list' and 'notes'.

### 'list' file format ###

One exact IPv4 or IPv6 prefix per line. The lines must be sort(1)'ed.

### 'notes' file format ###

Anything goes.

Example policy
--------------

See the ```golden-policy.iosxr.txt``` file for an example policy generated from
the list files.

