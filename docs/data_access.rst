******************
Data Access
******************

IATI tables transforms IATI data into relational tables, and provides multiple ways to access these data. 

`IATI Tables Datasette <https://datasette.tables.iatistandard.org/iati>`_
========================================================================

`Datasette  <https://datasette.io/>`_ is an open source tool for exploring data. 
The `IATI Tables Datasette <https://datasette.tables.iatistandard.org/>`_ instance allows you to explore IATI data your browser using SQL, 
and download the results of your query in multiple formats. You can also query IATI Tables Datasette from notebooks, such as Google Colab or Deepnote.

See the :ref:`Getting Started <gettingstarted>` section for tips on using IATI Tables Datasette.

For more information on the Datasette tool, see the `Datasette documentation <https://docs.datasette.io/en/stable/>`_.

`CSV Zip <https://tables.iatistandard.org/>`_
=================================================

The CSV Zip download is a compressed folder containing a CSV file for each table, which you can explore by importing into a spreadsheet viewer such as Excel or Google Sheets.
For more information, see :ref:`Spreadsheets <spreadsheets>`.

`SQLite Zip <https://tables.iatistandard.org/>`_
=================================================

The SQLite Zip download is a compressed `SQLite <https://www.sqlite.org/>`_ database, which can be run and explored with :code:`sqlite3`.

`PG Dump <https://tables.iatistandard.org/>`_
=================================================

The PG Dump download can be loaded into a `PostgreSQL <https://www.postgresql.org/>`_ database and are created by the `pg_dump <https://www.postgresql.org/docs/current/app-pgdump.html>`_ utility.

There are two options to choose from, gzip or custom:

Gzip 
    The 'gzip' format gives you a compressed plaintext script of SQL commands, which can be restored using :code:`psql`.

Custom
    The 'custom' format can be restored using the `pg_restore <https://www.postgresql.org/docs/current/app-pgrestore.html>`_ utility.   
    This option is more flexible if you want to perform any schema changes before restoring.