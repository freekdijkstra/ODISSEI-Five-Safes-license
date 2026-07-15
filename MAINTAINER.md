# Maintainer notes

Technical background and conventions for maintainers of this repository.


## Versioning

This repository defines three namespaces under `https://w3id.org/tre/`, each
versioned differently:

### Versioning in the `license` sub-namespace

The ODRL versioning follows the versioning of the authoritative text
versioning:

| Version | Text URL (=IRI)                         | ODRL URL                                             |
|---------|-----------------------------------------|------------------------------------------------------|
| Latest  | https://doi.org/10.5281/zenodo.18456774 | https://w3id.org/tre/license/five_safes_license      |
| 1.0.x   | https://doi.org/10.5281/zenodo.18456775 | https://w3id.org/tre/license/five_safes_license_v1.0 |

Changes in the textual represenation of the license will increase the major
version.

Changes in the ODRL representation of the license, without changes in the
textual representation will increase the minor version.

Patches to the ODRL that do not introduce new vocabulary will increase the
patch version.

### Versioning in the `vocabulary` sub-namespace

The vocabulary currently only uses a single digit versioning in the URL (and
IRI). This is currently "v0" to indicate the experimental nature.

`https://w3id.org/tre/vocabulary/v0#`

Backward compatible changes (such as addition of new concepts) will not
increase this version number.

For backward compatible changes to the file, see either the metadata or the
git history.

### Versioning in the `instance` sub-namespace

The URI (and IRI) of instance namespace remains unchanged; only the latest
version is published.

`https://w3id.org/tre/instance/sane#`

Updates will overwrite older versions.
For changes to the file, see either the metadata or the git history.


## w3id.org redirects

`w3id.org/tre/` URIs are resolved by rewrite rules maintained in a separate
repository: [github.com/perma-id/w3id.org/tree/master/tre/](https://github.com/perma-id/w3id.org/tree/master/tre/).

For the exact rewrite rules, including content negotiations, see the
[.htaccess](https://github.com/perma-id/w3id.org/blob/master/tre/.htaccess)
file in that repository.
