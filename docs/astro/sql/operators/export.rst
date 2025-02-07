.. _export_file:

====================
export_file operator
====================

.. _export_file_operator:

When to use the ``export_file`` operator
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The ``export_file`` function writes SQL table to csv/parquet on local/S3/GCS. The ``export_file`` function imports data from :ref:`supported_databases` or pandas dataframe.

There are two use cases of the ``export_file`` operator.


Case 1: Export file from table.
    The following example saves your :ref:`table` of data to file storage using the ``export_file``, which returns a pointer to File object.

    .. literalinclude:: ../../../../example_dags/example_google_bigquery_gcs_load_and_save.py
       :language: python
       :start-after: [START export_example_1]
       :end-before: [END export_example_1]

Case 2: Export file from dataframe.
    The following example saves your pandas dataframe of data to file storage using the ``aql.export_file``, which returns a pointer to File object.

    .. literalinclude:: ../../../../example_dags/example_google_bigquery_gcs_load_and_save.py
       :language: python
       :start-after: [START export_example_2]
       :end-before: [END export_example_2]
