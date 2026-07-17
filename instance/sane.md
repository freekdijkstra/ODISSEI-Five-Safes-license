# SANE Specification

IRI: `https://w3id.org/tre/instance/sane`

Namespace: `https://w3id.org/tre/instance/sane#` (prefix `sane:`)

Specification of the SANE Trusted Research Environment, provided by SURF.

Service defined in this schema: [SRC](#src).

Instances defined in this schema: [SANE](#sane), [Blind](#blind), [Tinker](#tinker).

## Service

### SRC

| Instance of `tre:TREService` | **sane:SRC** |
|:-----------------------------|:-------------|
| URI                          | `https://w3id.org/tre/instance/sane#SRC` |
| Label                        | SURF Research Cloud |
| Description                  | The SURF Research Cloud service, through which users can provision a SANE Trusted Research Environment. |
| Scope note                   | Only use sane:SRC in the context of a tre:TREService. It is not intended as an overall description of the SURF Research Cloud service. |
| Editorial note               | A general RDF description of the SURF Research Cloud service does not yet exist, as of 2026-07-17. |
| `schema:about`               | [https://surfresearchcloud.nl/](https://surfresearchcloud.nl/) |
| `schema:provider`            | [SURF](https://surf.nl) |
| `dpv:hasJurisdiction`        | `loc:NL` |
| `schema:serviceOutput`       | `sane:SANE` |

## Instances

### SANE

| Instance of `tre:TRE`, `odrl:RightOperand` | **sane:SANE** |
|:--------------------------------------------|:--------------|
| URI                                         | `https://w3id.org/tre/instance/sane#SANE` |
| Label                                       | SANE |
| Description                                 | SURF Secure Analysis Environment. A Trusted Research Environment (TRE) that allows analysis on a (confidential) dataset, without the data leaving the environment. The output is released after a check by the data provider. |
| Scope note                                  | Intended for use as the odrl:rightOperand of a Refinement/Constraint whose odrl:leftOperand is odrl:virtualLocation. |
| `schema:provider`                           | [SURF](https://surf.nl) |
| `dpv:hasLocation`                           | `loc:NL` |
| `dpv:hasDataProcessor`                      | [SURF](https://surf.nl) |
| `schema:potentialAction`                    | `tre:analyse` |

### Blind

| Instance of `tre:TRE`, `odrl:RightOperand` | **sane:Blind** |
|:--------------------------------------------|:---------------|
| URI                                         | `https://w3id.org/tre/instance/sane#Blind` |
| Label                                       | Blind SANE |
| Description                                 | Job submission system that runs code on a (confidential) dataset. The environment does not have Internet access, and the result of the analysis is send to the data provider for verification. |
| Scope note                                  | Intended for use as the odrl:rightOperand of a Refinement/Constraint whose odrl:leftOperand is odrl:virtualLocation. |
| `rdfs:subClassOf`                           | `sane:SANE` |
| `schema:provider`                           | [SURF](https://surf.nl) |
| `dpv:hasLocation`                           | `loc:NL` |
| `dpv:hasDataProcessor`                      | [SURF](https://surf.nl) |
| `schema:potentialAction`                    | `tre:analyse` |

### Tinker

| Instance of `tre:TRE`, `odrl:RightOperand` | **sane:Tinker** |
|:--------------------------------------------|:----------------|
| URI                                         | `https://w3id.org/tre/instance/sane#Tinker` |
| Label                                       | Tinker SANE |
| Description                                 | Remote desktop environment that provides tool to run an analysis on a (confidential) dataset. The environment does not have Internet access, and the result of the analysis is send to the data provider for verification. |
| Scope note                                  | Intended for use as the odrl:rightOperand of a Refinement/Constraint whose odrl:leftOperand is odrl:virtualLocation. |
| `rdfs:subClassOf`                           | `sane:SANE` |
| `schema:provider`                           | [SURF](https://surf.nl) |
| `dpv:hasLocation`                           | `loc:NL` |
| `dpv:hasDataProcessor`                      | [SURF](https://surf.nl) |
| `schema:potentialAction`                    | `tre:analyse` |

## Metadata

- License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- Creator: [SURF](https://surf.nl)
- Contributor: Freek Dijkstra
- Created: 2026-07-15
- Modified: 2026-07-17
- Machine-readable: [sane.ttl](sane.ttl), [sane.jsonld](sane.jsonld), [sane.rdf](sane.rdf) (XML)
