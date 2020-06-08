
========================
Pure functions reference
========================

Base function primitives implemented in functional programming paradigm.



Mnemonic(BIP39)
===============

.. autofunction:: pybfl.generate_entropy
.. autofunction:: pybfl.load_word_list
.. autofunction:: pybfl.entropy_to_mnemonic
.. autofunction:: pybfl.mnemonic_to_entropy
.. autofunction:: pybfl.mnemonic_to_seed


Private keys
============

.. autofunction:: pybfl.create_private_key
.. autofunction:: pybfl.private_key_to_wif
.. autofunction:: pybfl.wif_to_private_key
.. autofunction:: pybfl.is_wif_valid


Public keys
===========

.. WARNING::
   Using uncompressed public keys is
   `deprecated <https://github.com/bitcoin/bips/blob/master/bip-0143.mediawiki#restrictions-on-public-key-type>`_
   in  a new SEGWIT address format.
   To avoid potential future funds loss, users MUST NOT use uncompressed keys
   in version 0 witness programs. Use uncompressed keys only for backward
   compatibilitylegacy in legacy address format (PUBKEY, P2PKH).


.. autofunction:: pybfl.private_to_public_key
.. autofunction:: pybfl.is_public_key_valid



Extended keys(BIP32)
====================

.. autofunction:: pybfl.create_master_xprivate_key
.. autofunction:: pybfl.xprivate_to_xpublic_key
.. autofunction:: pybfl.derive_xkey
.. autofunction:: pybfl.public_from_xpublic_key
.. autofunction:: pybfl.private_from_xprivate_key



Addresses
=========

.. autofunction:: pybfl.hash_to_address
.. autofunction:: pybfl.address_to_hash
.. autofunction:: pybfl.public_key_to_address
.. autofunction:: pybfl.address_type
.. autofunction:: pybfl.address_to_script
.. autofunction:: pybfl.is_address_valid



Script
======

.. autofunction:: pybfl.decode_script
.. autofunction:: pybfl.parse_script
.. autofunction:: pybfl.delete_from_script
.. autofunction:: pybfl.script_to_hash


Signatures
==========

.. autofunction:: pybfl.verify_signature
.. autofunction:: pybfl.sign_message
.. autofunction:: pybfl.is_valid_signature_encoding


Hash encoding
=============

.. autofunction:: pybfl.rh2s
.. autofunction:: pybfl.s2rh
.. autofunction:: pybfl.reverse_hash


Merkle root
===========

.. autofunction:: pybfl.merkle_root
.. autofunction:: pybfl.merkle_branches
.. autofunction:: pybfl.merkleroot_from_branches


Difficulty
==========

.. autofunction:: pybfl.bits_to_target
.. autofunction:: pybfl.target_to_difficulty
.. autofunction:: pybfl.bits_to_difficulty
.. autofunction:: pybfl.difficulty_to_target


Tools
=====

.. autofunction:: pybfl.bytes_needed
.. autofunction:: pybfl.int_to_bytes
.. autofunction:: pybfl.bytes_to_int
.. autofunction:: pybfl.int_to_var_int
.. autofunction:: pybfl.var_int_to_int
.. autofunction:: pybfl.var_int_len
.. autofunction:: pybfl.get_var_int_len
.. autofunction:: pybfl.read_var_int
.. autofunction:: pybfl.read_var_list
.. autofunction:: pybfl.int_to_c_int
.. autofunction:: pybfl.c_int_to_int
.. autofunction:: pybfl.c_int_len






