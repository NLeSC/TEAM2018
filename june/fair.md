# Sprint Name

Fair-check -- FAIR Metrics Validator

# Team leader

Carlos / Arnold

# Target project

Develop tools for evaluating FAIRMetrics.

# Expertise required

 - Linked Data / RDF / Ontologies
 - Python
 - Docker

# Size of team

4 or 5

# Description

In the ecosystem of open science, [FAIR principles](https://www.dtls.nl/fair-data/fair-principles-explained/) are becoming increasingly important. [FAIRMetrics](http://fairmetrics.org) are seen as a way for FAIR principles to become more widely implemented in a concrete sense. According to the [JISC report](https://zenodo.org/record/1245568#.WxUq1HWFNhE) on FAIR data principle in practice, one of the current barriers found is `Current lack of metrics and measures to assess FAIRness led to inconsistent views on adherence to FAIR`.

The aim of this team would be to implement a system to automatically evaluate compliance to FAIRMetrics of a given resource.

The ultimate aim of this team would be to contribute our implementation upstream to the [FAIRMetrics](https://github.com/FAIRMetrics/Metrics/).

As a concrete usecase, the [Interstellar](https://github.com/NLeSC/TEAM2018/blob/master/june/interstellar.md) data could be used.

# Goals

 - Develop awareness of the latest developments done at [FAIRMetrics](https://github.com/FAIRMetrics/Metrics/)
 - Develop a python package capable of measuring FAIRMetrics automatically and produce a compliance score.
 - Example code could look something like this:

```python
import FAIRMetrics
myMetrics = FAIRMetrics({
  'F': [ 'http://uri-for-F-metric'], # EG: https://purl.org/fair-metrics/FM-F1A
  'A': [ 'http://uri-for-A-metric'],
  'I': [ 'http://uri-for-I-metric'],
  'R': [ 'http://uri-for-R-metric']
})
myResource = 'http://uri-of-target-resource' # eg. Xenon DOI: https://doi.org/10.5281/zenodo.1200251

score = myMetrics.evaluate(myResource)
```
