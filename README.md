EWP Statistics Gathering API
==========================================

* [What is the status of this document?][statuses]
* [See the index of all other EWP Specifications][develhub]


Summary
-------

This document describes the **Statistics Gathering API**.
This API allows HEIs to share different statistics about their [Learning Agreements][las-api] and Interinstitutional Agreements [Interinstitutional Agreements API][iias-api].

Request method
--------------

 * Requests MUST be made with either HTTP GET or HTTP POST method. Servers MUST
   support both these methods. Servers SHOULD reject all other request methods.


Security
--------

This version of this API uses [standard EWP Authentication and Security, Version 2][sec-v2].
Server implementers choose which security methods they support by declaring them
in their Manifest API entry.


Handling of invalid parameters
------------------------------

 * General [error handling rules][error-handling] apply.

Response
--------

Servers MUST respond with a valid XML document described by the
[response.xsd](response.xsd) schema. See the schema annotations for further
information.

Examples
--------

An example SQL queries needed to gather these statistics fur USOS database can be found [here][github-issue] repository.


[develhub]: http://developers.erasmuswithoutpaper.eu/
[error-handling]: https://github.com/erasmus-without-paper/ewp-specs-architecture#error-handling
[iias-api]: https://github.com/erasmus-without-paper/ewp-specs-api-iias
[las-api]: https://github.com/erasmus-without-paper/ewp-specs-api-omobility-las
[statuses]: https://github.com/erasmus-without-paper/ewp-specs-management#statuses
[github-issue]: https://github.com/erasmus-without-paper/ewp-specs-api-omobility-las/issues/37
[sec-v2]: https://github.com/erasmus-without-paper/ewp-specs-sec-intro/tree/stable-v2
