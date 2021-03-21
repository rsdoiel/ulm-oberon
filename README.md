Ulm Oberon
==========

Ulm Oberon is a compiler and set of tools for working
in Oberon obtained from Andres Borchert's website
at http://www.mathematik.uni-ulm.de/oberon/ on
2021-03-21 by me.  Since many oberon related projects
are disappearing from the web I thought it prudent to
create this archive of Ulm Oberon compiler. The
website has been archived at [archive.org](https://web.archive.org/web/2020*/https://www.mathematik.uni-ulm.de/oberon/)

Ulm Oberon i386-0.8.10
----------------------

Ulm Oberon compiler has features of Oberon 2
as well as some from Oberon 1. Notible is
the use of separate definition files. The files
with extension of ".od" are the definition and
the ".om" are the Oberon modules. 

The material was obtained with the following
commands on 2021-03-21 and setup as a git
repository.

```shell
    mkdir ulm-oberon
    cd ulm-oberon
    cat <<EOT > .gitignore
*.gz
*~
*.tmp
*.swp
EOT
    wget "http://www.mathematik.uni-ulm.de/oberon/ftp/i386/READ_ME"
    wget "http://www.mathematik.uni-ulm.de/oberon/ftp/i386/examples/ReverseIPv4.od"
    wget "http://www.mathematik.uni-ulm.de/oberon/ftp/i386/examples/ReverseIPv4.om"
    wget "http://www.mathematik.uni-ulm.de/oberon/ftp/i386/ulm-oberon-i386-0.8.10.tar.gz"
    tar zxvf ulm-oberon-i386-0.8.10.tar.gz
    git init
    git add .
    git commit -am "Initial Archive"
    git branch -M main
```

From here you can then push to your favorite Git host (e.g. GitHub,
Bitbucket, Gitlab)




There are SPARC and sun3 versions of the compiler
but I didn't archive those because I have no access
to that hardware.


