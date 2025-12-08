******************
Data Retrieval
******************

This section outlines how IATI data is retrieved by IATI Tables.

Data Source
============

IATI Tables retrieves a daily snapshot of all IATI data from the `IATI Bulk Data Service <https://bulk-data.iatistandard.org/>`_.
All data is replaced each time the process runs, so updates and removals are respected.

The `metadata table <https://datasette.codeforiati.org/iati/metadata>`_ shows the cut-off time for data to be included.
The column :code:`iati_tables_updated_at` shows the time at which the tables run finished.
The column :code:`data_dump_updated_at` shows the time of the Bulk Data Service snapshot that was used by the latest run.
IATI data published or edited after this time will not be included in IATI Tables until the next run.
