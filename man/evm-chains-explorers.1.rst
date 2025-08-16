..
   SPDX-License-Identifier: AGPL-3.0-or-later

   ----------------------------------------------------------------------
   Copyright © 2024, 2025  Pellegrino Prevete

   All rights reserved
   ----------------------------------------------------------------------

   This program is free software: you can redistribute it and/or modify
   it under the terms of the GNU Affero General Public License as published by
   the Free Software Foundation, either version 3 of the License, or
   (at your option) any later version.

   This program is distributed in the hope that it will be useful,
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU Affero General Public License for more details.

   You should have received a copy of the GNU Affero General Public License
   along with this program.  If not, see <https://www.gnu.org/licenses/>.


============================
evm-chains-explorers
============================

----------------------------------------------------------------------
Ethereum Virtual Machine (EVM) compatible network explorers manager
----------------------------------------------------------------------
:Version: evm-chains-explorers |version|
:Manual section: 1

Synopsis
========

evm-chains-info *[options]* *command* *key* (*value*)

Description
===========
Returns info about Ethereum Virtual Machine (EVM)
compatible blockchains explorers.


Commands
=========

* get
    *key*
      *value*



Keys
=====

* key                        Given an explorer as value returns
                             the path of its available API keys.
* keys                       Shows all available API keys for
                             target blockchain's explorers.
* keys_explorers             Shows all explorers for which
                             API keys are available.


Values
========

* explorer

Options
========

-c target_chain         Target chain for which to return
                        explorer informations. Valid
                        values are all those accepted by
                        evm-chains-info.
-s selection_method     When output type is 'rpc', 
                        selection criterion to use when
                        more than one is available.
                        It can be 'kirsh', 'random' or
                        'all'.

-h                      Displays help.
-c                      Enable color output
-v                      Enable verbose output

Bugs
====

https://github.com/themartiancompany/evm-chains-explorers/-/issues

Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.

See also
========

* evm-chains-info
* evm-chains-explorers
* evm-contract-call
* evm-wallet

.. include:: variables.rst
