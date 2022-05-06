Usage.restAPI
=====

Helpful Endpoints for:


.. _installation:

General
------------

``Check`` Balance Started when begin CopyTrade:

.. code-block:: console

   GET /apiBom/balancestart/<cust_name>
   

``Check`` Profit And Loss (report):

.. code-block:: console

   GET /apiBom/reportpnl/<cust_name>


``Check`` Transfer/Deposit/Withdrawal:

.. code-block:: console

   GET /apiBom/transactionhistory/<cust_name>
Binance Futures
------------


``Check`` CopyTrade's data (master/slave):

.. code-block:: console

   GET /apiBom/ft/master/<cust_name>
   GET /apiBom/ft/slave/<cust_name>


   
``Check`` your info in the CopyTrade system:

.. code-block:: console

   is under active development.
   
``Check`` Balance:

.. code-block:: console

   GET /apiBom/ft/balance/<cust_name>
   GET /fapi/v2/balance (HMAC SHA256)  *From Binance API: Futures Account Balance V2 (USER_DATA)

  
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

   
``Check`` your info in the CopyTrade system:

.. code-block:: console

   is under active development.
   
``Check`` Balance:

.. code-block:: console

   is under active development.
   OR: GET /api/v3/account (HMAC SHA256)  *From Binance Spot/Margin/Savings/Mining's API: Account Information (USER_DATA)

  
``CANCEL`` Open Orders:

.. code-block:: console

   is under active development.
   
``SELL`` your Coin:

.. code-block:: console

   is under active development.
   
   
``CASH OUT ALL COINS TO USDT``:

.. code-block:: console

   is under active development.
   
``UPDATE`` your capital per trade order:

.. code-block:: console

   is under active development.

API status/logs
----------------

``Check`` API's status || Logs:

.. code-block:: console

   GET /apiBom/status/ft/<cust_name>
   GET /apiBom/status/spot/<cust_name>
   GET /apiBom/logs/<cust_name>

👀 If you have any bugs or questions on how to use it, have a look at `Gambling X-Group <https://t.me/+U6w16xyWcSAUD7Y9/>`_, or head to  `@Cuongitl <https://t.me/Cuongitl/>`_
