# ODISSEI Five Safes license

IRI: `https://w3id.org/tre/license/five_safes_license`

Namespace: `https://w3id.org/tre/license/` (prefix `fsl:`)

ODRL version of a standardised set of conditions for accessing and using sensitive datasets in a Trusted Research Environment (TRE) such as SANE, according to the Five Safes principles.

Scope note: To refer to version 1 of the Five Safes License, use the Zenodo identifier, also for ODRL parsing.

This is version 1.1.0 of the ODRL version, which corresponds to version v1.01 of the text version, available at [Zenodo](https://doi.org/10.5281/zenodo.18456775).

## Conditions

| Type       | Term         | Details      |
|:-----------|:-------------|:-------------|
| Action     | `fsl:action-analyse-in-sane` | `tre:analyse`, refined to only inside `sane:SANE` |
| Assignee   | `fsl:assignee-odissei-member` | member of ODISSEI (`odrl:source <https://odissei-data.nl/>`) |
| Assignee   | `fsl:assignee-located-europe-economic-area` | located in the European Economic Area (`odrl:spatial isAnyOf loc:EEA`) |
| Assignee   | `fsl:assignee-affiliation-employee-faculty` | eduPersonAffiliation is "employee" or "faculty" |
| Constraint | `fsl:constraint-elapsed-time` | access expires after 3 months (`odrl:elapsedTime lteq "P3M"`) |
| Duty       | `fsl:duty-attribution` | attribute the dataset (`odrl:attribute`) |
| Duty       | `fsl:duty-declare-purpose-non-commercial` | declare intended purpose, restricted to `dpv:NonCommercialResearch` |
| Duty       | `fsl:duty-accept-terms` | accept the terms of use (`tre:acceptTerms`) |
| Prohibition | - | redistribution (`odrl:distribute`) is prohibited. |

## Metadata

- Version: 1.1.0
- Version IRI: https://w3id.org/tre/license/five_safes_license_v1.1
- License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- Creator: [SURF](https://surf.nl), [ODISSEI](https://odissei-data.nl)
- Contributor: Freek Dijkstra, Lucas van der Meer
- Created: 2026-02-25
- Modified: 2026-07-17
- Machine-readable: [five_safes_license.ttl](five_safes_license.ttl), [five_safes_license.jsonld](five_safes_license.jsonld), [five_safes_license.rdf](five_safes_license.rdf) (XML)
