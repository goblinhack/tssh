tssh
====

Multi threaded ssh of a large file to a destination. Uses checksums for 
incremental speedups on subsequent copies.

Example:

  $ tssh -t 20 -d -v bigfile user@farawayhost:/path/bigfile

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

