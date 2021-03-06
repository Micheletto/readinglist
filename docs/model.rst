##########
Data model
##########

.. _data-model:

Articles
========

+--------------------+-------------+----------------------------------+
| Attribute          | Type        | Comment                          |
+====================+=============+==================================+
| ``id``             | UUID        |                                  |
+--------------------+-------------+----------------------------------+
| ``last_modified``  | Timestamp   | server timestamp                 |
+--------------------+-------------+----------------------------------+
| ``url``            | URL         | valid (RFC)                      |
+--------------------+-------------+----------------------------------+
| ``preview``        | URL         | feature image URL                |
+--------------------+-------------+----------------------------------+
| ``title``          | String(1024)| 1 character min.                 |
+--------------------+-------------+----------------------------------+
| ``resolved_url``   | URL         | after potential redirections     |
+--------------------+-------------+----------------------------------+
| ``resolved_title`` | String(1024)| extracted from target page       |
+--------------------+-------------+----------------------------------+
| ``excerpt``        | Text        | first 200 words of the article   |
+--------------------+-------------+----------------------------------+
| ``archived``       | Boolean     |                                  |
+--------------------+-------------+----------------------------------+
| ``favorite``       | Boolean     |                                  |
+--------------------+-------------+----------------------------------+
| ``is_article``     | Boolean     | false if no textual content      |
+--------------------+-------------+----------------------------------+
| ``word_count``     | Integer     |                                  |
+--------------------+-------------+----------------------------------+
| ``unread``         | Boolean     |                                  |
+--------------------+-------------+----------------------------------+
| ``added_by``       | Device      | device name (cf. issue #23)      |
+--------------------+-------------+----------------------------------+
| ``added_on``       | Timestamp   | device timestamp                 |
+--------------------+-------------+----------------------------------+
| ``stored_on``      | Timestamp   | server timestamp                 |
+--------------------+-------------+----------------------------------+
| ``marked_read_by`` | Device      | device name (cf. issue #23)      |
+--------------------+-------------+----------------------------------+
| ``marked_read_on`` | Timestamp   | device timestamp                 |
+--------------------+-------------+----------------------------------+
| ``read_position``  | Integer     | Words read from the beginning    |
+--------------------+-------------+----------------------------------+
