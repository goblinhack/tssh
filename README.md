tssh
====

Multi threaded ssh of a large file to a destination. Uses checksums for 
incremental speedups on subsequent copies.

  $ tssh [-t x] [-u user] src host dest

  $ tssh [-t x] [-u user] src host:dest

  $ tssh [-t x] [-u user] src user@host:dest

Defaults to 10 threads. Options:

      -threads
      --threads
      -t  ... How many scp threads to run

      -quiet
      --quiet
      -q  ... Quiet, no logging to console

      -user
      --user
      -u  ... Username

      -debug
      --debug
      -d  ... Debug

      -help
      --help
      -h  ... Help

      -verify
      --verify
      -v  ... Check results

Example:

  $ tssh -t 20 -d -v file admin@rtp-xdm-104:/auto/rtp-core-tftpboot/nmcgill/file
