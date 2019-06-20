## Current status: DRAFT, work in progress

Please consider this work as non-final for the time being.

## This repository

This repository contains an XML Schema for entities defined in the EBU-TT Metadata specification,
[Tech3390](https://tech.ebu.ch/publications/tech3390).

* Copyright 2019, EBU, www.ebu.ch
* Version of XML Schema: 0.9
* Creation: 24/05/2019

The publication of this EBU-TT XML Schema for EBU-TT Metadata is intended to support the 
implementation of the specification in EBU-Tech 3390 version 1.0.

Please note that the EBU-TT XML Schema is a helping document and NOT normative but informative.

## Schema strictness

This repository includes two top level schema documents:
* `ebu-tt-metadata.xsd` defines metadata types for use in various TTML elements applying strict
validation to _should_ specifications in Tech3390 or other EBU-TT specifications, for
example restricting the use of `ebuttm:facet` to `ttm:metadata` elements that can be children of
content elements, and the use of `ebuttm:documentFacet` to the metadata child of the head
element.
* `ebu-tt-metadata-relaxed.xsd` defines all the metadata elements specified in Tech3390
and allows any of them to be used on any `ttm:metadata` element in any order, applying no
further constraints except that the deprecated element `ebuttm:documentMetadata` is not
permitted.

