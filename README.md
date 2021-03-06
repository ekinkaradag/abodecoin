*This is not an actual crypto-currency for real-world use. The nodes are neither created nor defined. This is just a demonstration for future possibilities*

 - Copyright (c) 2009 Bitcoin Developers
 - Copyright (c) 2011 Litecoin Developers
 - Copyright (c) 2018 Ekin Karadag

What is Abode Coin (ABC)?
----------------

Abode Coin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm. Abode Coin is an experimental digital currency that enables instant payments to anyone, anywhere in the world. Abodecoin uses peer-to-peer technology to operate with no central authority: managing transactions and issuing money are carried out collectively by the network. Abode Coin is the name of open source software which enables the use of this currency.
 - 5 minute block targets
 - Subsidy is 50 ABC
 - Subsidy halves in 630k blocks
 - There can only be a maximum of 63 million ABC
 - The wallet addresses start with "A" (testnet wallet addresses start with "a")

License
-------

Abode Coin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

If it is a simple/trivial/non-controversial change, then I simply pull it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/ekinkaradag/abodecoin/tags) are created
regularly to indicate new official, stable release versions of Abodecoin.

Testing
-------


### Automated Testing

Testing the code highly encouraged. Please be advised.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./abodecoin-qt_test

