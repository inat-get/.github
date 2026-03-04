# 🌿 iNatGet Project

## [inat-get](https://github.com/inat-get/inat-get)

<img src="./logo.webp" align="right" style="float:right;width:35%;">

*CLI tool for downloading and analyzing iNaturalist biodiversity data*

`inat-get` is a command-line interface for working with iNaturalist data, implemented in Ruby. The tool enables users to programmatically retrieve observation records from the iNaturalist platform and process them for research and analysis purposes.

Key capabilities include downloading observations based on taxonomic, geographic, and temporal filters; exporting data in multiple formats for integration with analytical workflows; and generating summary statistics from biodiversity datasets. `inat-get` is designed to facilitate reproducible data collection from iNaturalist, supporting research in ecology, conservation biology, phenology, and related fields.

## [inat-channel](https://github.com/inat-get/inat-channel)

*Script for posting selected observation to telegram channel*

A script that sends a random iNaturalist observation from a selected sample to Telegram.

+ Obtains a sample via the [iNaturalist API](https://api.inaturalist.org/v2/docs/#/Observations/get_observations) based on an arbitrary query (supported by the API).

+ Sends a random observation from the sample to a specified Telegram channel, excluding those already sent. If there are no new observations in the fresh sample, it takes from a saved pool.

+ Saves unsent observations obtained via the query into the pool.

+ Taxon uniqueness and pool depth are configurable.

+ Sends a message to the administrator in case of failures.
