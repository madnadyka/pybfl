.. aiohttp documentation master file, created by
   sphinx-quickstart on Wed Mar  5 12:35:35 2014.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

==================
Welcome to pybfl
==================

Python library for Bitflate.

Current version is 2.0.


.. _GitHub: https://github.com/pybfl/pybfl


Key Features
============


- Supports addresses types PUBKEY, P2PKH, P2SH, P2SH-PWPKH, P2WPKH, P2WSH.
- Supports BIP32(Hierarchical Deterministic Wallets), BIP39(Mnemonic code generation)
- Supports BIP141(Segregated Witness)
- Transaction constructor
- Mining pool basic primitives


Getting Started
===============

Usage example::

    import pybfl
    a = pybfl.Address()
    print(a.address)
    print(a.private_key.wif)


Dependencies
============

- Python 3.3.3+
- *secp256k1*




Table Of Contents
=================

.. toctree::
   :name: mastertoc
   :maxdepth: 2

   installation.rst
   examples.rst
   classes.rst
   functional.rst
   contributing.rst



