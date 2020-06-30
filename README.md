# ec-earth-errata-tracer

The [ES-DOC errata](https://errata.es-doc.org/static/index.html) is the official platform which lists all CMIP6 related errata for CMIP6 model output. When selecting at this page `EC-EARTH-CONSORTIUM` in the drop-down menu of the`Institution ID` column, all EC-Earth3 related ES-DOC reported errata are listed. However, because in practice often it takes a while before official ES-DOC errata are published, we launched this public Github errata tracer platform in order to track and trace EC-Earth related issues concerning the CMIP6 output which has been published on the ESGF nodes.

A part of the CMIP6 output errata issues is related to the EC-Earth post processing ([ece2cmor3](https://github.com/EC-Earth/ece2cmor3/)) and some are related to an issue in EC-earth3 but can be addressed in the post processing. In some cases we are able to correct the data without recmorising but by applying the [cmor-fixer](https://github.com/EC-Earth/cmor-fixer/) on the cmorised data directly. For instance the `cmor-fixer` has been used by the ESGF data managers in order to correct EC-Earth3 data on the ESGF nodes, avoiding any further large volume data transfer.

EC-Earth3 CMIP6 output issues which are related to [ece2cmor3](https://github.com/EC-Earth/ece2cmor3/) are reported at an `ece2cmor3` wiki [EC-Earth3-ESGF-errata page](https://github.com/EC-Earth/ece2cmor3/wiki/EC-Earth3-ESGF-errata). However, this table does not list errata issues which are caused by a mistake by a data producer: For instance when incorrect metadata is published like an incorrect `branch_time` or an incorrect ensemble member name. Note that the `cmor-fixer` has an option to correct for such metadata issues as well.

This `ec-earth-errata-tracer` platform can be used to report any EC-Earth3 CMIP6 output issue encountered on the ESGF nodes immediately and to trace the status. Partly this will concern links to the `cmor-fixer` and to `ece2cmor3` which are both public assesible, at the other hand it will refer to EC-Earth issues on the non-public EC-Earth portal which is only open to the EC-Earth community.

At this `ec-earth-errata-tracer` platform we will open issues and trace them by a certain status:
* new reported
* issue confirmed | issue not confirmed
* ES-DOC erratum created
* wil be fixed | won't be fixed
* implementing a fix
* fix ready
* fix applied
* ES-DOC erratum closed

