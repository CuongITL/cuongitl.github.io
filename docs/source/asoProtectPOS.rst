💥Automated System Operations (ASO)

AutoTrade Protect your Positions with fee 2$/day
=====

Features:
------------

- Auto Take-profit your postion when MarkPrice hit ROE% by setting.

- Auto DCA your postion when MarkPrice hit ROE% by setting.

Usage.Telegram Bot
------------

``Check`` your settings:

.. code-block:: console

   /bcz <cust_name>


``CHANGE`` your settings:

.. code-block:: console

  /bcz <action> <value>
  
Example 1: change maxMargin = 50$
 
 .. code-block:: console

   /bcz maxMargin 50

Example 2: change DCA at ROE = 80%
 
 .. code-block:: console

   /bcz roe 80
 
Example 3: change DCA's multi(martingale) = 1.5
 
 .. code-block:: console

   /bcz multi 1.5


Example 4: change tpRR = 1.2
 
 .. code-block:: console

   /bcz tpRR 1.2


Example 5: add a coin to skip_protect_list
 
 .. code-block:: console

   /bcz add LUNAUSDT



Example 6: remove a coin from skip_protect_list
 
 .. code-block:: console

   /bcz remove LUNAUSDT

===============
‼️  Action: ['maxMargin', 'roe', 'multi', 'tpRR', 'add', 'remove']
