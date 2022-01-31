==================================
kissbom: The keep it simple SBoM
==================================

Context and Problem
--------------------

Reporting software provenance to track licensing, bugs and
vulnerabiilities is useful.

What could be the simplest way to craft a Software Bill
of Material (SBoM)?

Solution
---------

A kissbom is a document that lists all the software packages
included in the software it documents, both own code and
third-party.

The attributes for each item in this list are: 

- purl: a Package URL string.
- license: an optional SPDX license expression string.
- copyright: an optional copyright holder name(s) string.
- notes: an optional notes string.

These attributes are sufficient to:

- document packages provenance and license,
- query package details from repositories, including dependencies,
- download packages, and
- query bug trackers and vulnerability databases for package issues.

purl and SPDX license expressions have their own spec.

The extensions for kissbom files are ".kissbom.json", ".kissbom.yml",
".kissbom.csv", etc.

The filename should be used to document the subject of the SBoM
including optionally the product or component name, the SBoM author
name, and an ISO 8601 timestamp of when this SBoM was last modified.
Filenames should be lowercase and contain no space and should
prefer using "-",  "_" and "." as separator between words.

Content is UTF-8-encoded and can be serialized as JSON, YAML, CSV or
any other format. 
