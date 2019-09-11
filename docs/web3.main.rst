Web3 API
========

.. contents:: :local:

.. py:module:: web3
.. py:currentmodule:: web3


.. py:class:: Web3(provider)

Each ``web3`` instance exposes the following APIs.

Providers
~~~~~~~~~

.. py:attribute:: Web3.HTTPProvider

    Convenience API to access :py:class:`web3.providers.rpc.HTTPProvider`

.. py:attribute:: Web3.IPCProvider

    Convenience API to access :py:class:`web3.providers.ipc.IPCProvider`

.. py:method:: Web3.setProviders(provider)

    Updates the current web3 instance with the new list of providers. It
    also accepts a single provider.


Attributes
~~~~~~~~~~

.. py:attribute:: Web3.api

    Returns the current Web3 version.

    .. code-block:: python
     
       >>> web3.api
       "4.7.0"

.. py:attribute:: Web3.clientVersion

    * Delegates to ``web3_clientVersion`` RPC Method

    Returns the current client version.

    .. code-block:: python

       >>> web3.clientVersion
       'Geth/v1.4.11-stable-fed692f6/darwin/go1.7'


Encoding and Decoding Helpers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

See :ref:`overview_type_conversions`


Currency Conversions
~~~~~~~~~~~~~~~~~~~~~

See :ref:`overview_currency_conversions`


Addresses
~~~~~~~~~

See :ref:`overview_addresses`


RPC APIS
--------

Each ``web3`` instance also exposes these namespaced APIs.


.. py:attribute:: Web3.eth

    See :doc:`./web3.eth`

.. py:attribute:: Web3.miner

    See :doc:`./web3.miner`

.. py:attribute:: Web3.pm

    See :doc:`./web3.pm`

.. py:attribute:: Web3.geth

    See :doc:`./web3.geth`

.. py:attribute:: Web3.parity

    See :doc:`./web3.parity`
