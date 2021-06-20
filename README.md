Timecoin integration/staging tree
================================

http://www.timecoin.center

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Litecoin Developers
Copyright (c) 2021 Timecoin Developers

What is Timecoin?
----------------
Time Coin the currency for the Timecoin Community. Once member obtained Timecoin, they are free to use it to exchange services with other member of the community. We believe everyone's time is becoming more valuable over the time... So as the value of Timecoin. We know there will be interest for currency, we call it the time value of money. What will the time value of time be? We expect it grow even faster than currency.

Be the bridge between the virtual and reality. 

Use the virtual world to empower the possible change to a better world.

Parameters:
 - subsidy runs out in 2178.3 years. 
 - The number comes from mathematical constant e = 2.7183...
 - 75852041790 total coins.
 - The number comes from the total world population 7585204179.
 - 22 seconds block targets

For more information, as well as binary version of the Timecoin client sofware, see http://www.timecoin.center.

License
-------

Timecoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Timecoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/timecoin-project/timecoin/tags) are created
regularly to indicate new official, stable release versions of Timecoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./timecoin-qt_test

