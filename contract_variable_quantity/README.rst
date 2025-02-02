=================================================
Variable quantity in contract recurrent invoicing
=================================================

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:bf5c154ac65588fc280046147b7f3d978557cfe2cd62bd08acf47761e173da74
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fcontract-lightgray.png?logo=github
    :target: https://github.com/OCA/contract/tree/17.0/contract_variable_quantity
    :alt: OCA/contract
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/contract-17-0/contract-17-0-contract_variable_quantity
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/contract&target_branch=17.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

With this module, you will be able to define in recurring contracts some
lines with variable quantity according to a provided formula.

**Table of contents**

.. contents::
   :local:

Configuration
=============

1. Go to Invoicing > Configuration > Contracts > Formulas (quantity).

2. Define any formula based on Python code that stores at some moment a
   float/integer value of the quantity to invoice in the variable
   'result'.

   You can use these variables to compute your formula:

   -  *env*: Environment variable for getting other models.
   -  *context*: Current context dictionary.
   -  *user*: Current user.
   -  *line*: Contract recurring invoice line that triggers this
      formula.
   -  *contract*: Contract whose line belongs to.
   -  *invoice*: Invoice (header) being created.

|image1|

.. |image1| image:: https://raw.githubusercontent.com/OCA/contract/17.0/contract_variable_quantity/images/formula_form.png

Usage
=====

To use this module, you need to:

1. Go to Invoicing > Customers > Customers Contracts and select or
   create a new contract.
2. Check *Generate recurring invoices automatically*.
3. Add a new recurring invoicing line.
4. Select "Variable quantity" in column "Qty. type".
5. Select one of the possible formulas to use (previously created).

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/contract/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/contract/issues/new?body=module:%20contract_variable_quantity%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
-------

* Tecnativa

Contributors
------------

-  `Tecnativa <https://www.tecnativa.com>`__:

      -  Pedro M. Baeza
      -  Carlos Roca
      -  Víctor Martínez
      -  Carolina Fernandez
      -  Juan José Seguí

-  Dave Lasley <dave@laslabs.com>

-  Souheil Bejaoui <souheil.bejaoui@acsone.eu>

Maintainers
-----------

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/contract <https://github.com/OCA/contract/tree/17.0/contract_variable_quantity>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
