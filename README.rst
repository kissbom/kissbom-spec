==================================
kissbom: The keep it simple SBoM
==================================

Context and Problem
--------------------

Reporting software provenance and track licensing, bugs and
vulnerabiilities is useful.

What could be the simplest way we could do this?

Solution
---------

The kissbom is a document that lists all the software packages
included in the software it documents, both own code and
third-party.

The attributes for each items of this list are: 

- purl: a Package URL string.
- license: an optional SPDX license expression string.
- copyright: an optional copyright holder name(s) string.
- notes: an optional notes string.

purl and SPDX license expressions have their own spec.

Content is UTF-8-encoded and can be seralized as JSON, YAML, CSV or
any other format. 

The extensions for KISS BOM files are ".kissbom.json", ".kissbom.yml",
".kissbom.csv", etc.

The provided attributes are sufficient to:

- lookup package details, including dependencies from package repositories,
- download packages, and
- query bug trackers and vulnerability databases for issues.
