# dstar-sorcerer

building
----
    zcc +srr -lndos -create-app dstar.c -Cz--audio

installing z88dk
----
    wget http://nightly.z88dk.org/z88dk-latest.tgz
    tar -xzf z88dk-latest.tgz
    sudo apt-get install libxml2-dev
    sudo apt-get install m4
    cd z88dk/
    chmod 777 build.sh
    ./build.sh

You may need to tap return a few times if the build stalls!

Now update your environment to use the tools:
    vi ~/.bash_profile

Add the following to the end of the file:
    export PATH=${PATH}:${HOME}/z88dk/bin
    export ZCCCFG=${HOME}/z88dk/lib/config
