MODIFIED BY JEREMY TO MAKE EASIER TO RUN

I used virtual env wrapper: https://virtualenvwrapper.readthedocs.io/en/latest/

If no virtual env exists, create one with:

    $ mkvirtualenv mnemonic

If it does, then run it with

    $ workon mnemonic
    $ python setup.py develop

Close the virtualenv session to return to system python

    $ deactivate

To run type

    $ python mnemonic.py [16 digit hex string]

such as

    $ python mnemonic.py f2f2f2f2f2f2f2f2f2f2f2f2f2f2f2f2

===========

python-mnemonic
===============

.. image:: https://travis-ci.org/trezor/python-mnemonic.svg?branch=master
    :target: https://travis-ci.org/trezor/python-mnemonic

Reference implementation of BIP-0039: Mnemonic code for generating
deterministic keys

Abstract
--------

This BIP describes the implementation of a mnemonic code or mnemonic sentence --
a group of easy to remember words -- for the generation of deterministic wallets.

It consists of two parts: generating the mnenomic, and converting it into a
binary seed. This seed can be later used to generate deterministic wallets using
BIP-0032 or similar methods.

BIP Paper
---------

See https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki
for full specification
