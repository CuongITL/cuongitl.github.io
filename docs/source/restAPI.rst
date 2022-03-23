Usage.restAPI
=====

Helpful Endpoints for:


.. _installation:

Login/Register
------------


.. code-block:: console

   POST /apiBom/register
   POST /apiBom/login
   
   
Binance Futures
------------


``Check`` CopyTrade's data (master/slave):

.. code-block:: console

   GET /apiBom/ft/master/<cust_name>
   GET /apiBom/ft/slave/<cust_name>

``Check`` Profit And Loss (report):

.. code-block:: console

   GET /apiBom/ft/pnl/<cust_name>
   
``Check`` your info in the CopyTrade system:

.. code-block:: console

   is under active development.
   
``Check`` Balance:

.. code-block:: console

   GET /apiBom/ft/balance/<cust_name>

  
``CANCEL`` Open Orders:

.. code-block:: console

   is under active development.
   
``CLOSE`` your Positions:

.. code-block:: console

   is under active development.
   
``UPDATE`` your capital per trade order:

.. code-block:: console

   is under active development.


Binance Spot
----------------

``Check`` CopyTrade's data (master/slave):

.. code-block:: console

   GET /apiBom/spot/master/<cust_name>
   GET /apiBom/spot/slave/<cust_name>

``Check`` Profit And Loss (report):

.. code-block:: console

   GET /apiBom/spot/pnl/<cust_name>
   
``Check`` your info in the CopyTrade system:

.. code-block:: console

   is under active development.
   
``Check`` Balance:

.. code-block:: console

   is under active development.

  
``CANCEL`` Open Orders:

.. code-block:: console

   is under active development.
   
``CLOSE`` your Positions:

.. code-block:: console

   is under active development.
   
``UPDATE`` your capital per trade order:

.. code-block:: console

   is under active development.

API status
----------------

``Check`` API's CopyTrade:

.. code-block:: console

   GET /apiBom/status/<cust_name>


👀 If you have any bugs or questions on how to use it, have a look at my group (https://t.me/+U6w16xyWcSAUD7Y9/), or head to @Cuongitl.
