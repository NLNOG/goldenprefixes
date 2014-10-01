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
are present: ```list``` and ```notes```.

### 'list' file format ###

One exact IPv4 or IPv6 prefix per line. The list files must be piped through ```sort -n``` before changes are submitted.

### 'notes' file format ###

Anything goes.

### 'auth' file format ###

If a hmproject participant opts to PGP sign their 'list' file, consumers of the
hmproject data are required to validate the signature file associated with the
list file. In the ```auth``` file each line represents an ASN followed by one
or more PGP keys, delimited by spaces. The ```auth``` file itself is signed by
Job Snijders <job@ntt.net> and Jared Mauch <jared@puck.nether.net>. All PGP
signatures are detached and ASCII armored.

Example policy
--------------

See the ```golden-policy.iosxr.txt``` file for an example policy generated from
the list files.

