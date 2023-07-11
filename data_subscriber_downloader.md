# Bulk Data Subscriber and Download Service

This tutorial will demonstrate the utilization of a commandline-based tool known as the **podaac-data-subscriber[downloader]** which allows users to either subscribe to datasets (for periodic, continuous updating featuring the latest available data) or one-time "bulk" downloading of one or more data files with a single request.  

While originally developed by the [PO.DAAC](https://podaac.jpl.nasa.gov/), the **podaac-data-subscriber[downloader]** has recently been upgraded to enable access to data from other NASA Distributed Active Archive Centers (DAACs). For the purposes of this tutorial, we will simply demonstrate data access and extraction of TROPESS data from the NASA GES DISC using the one-time **downloader** feature. 

More specific details regarding the **podaac-data-subscriber[downloader]** can be found here: https://github.com/podaac/data-subscriber

You may also click the following links for more detailed documentation regarding the following options:
  1. [Subscriber](https://github.com/podaac/data-subscriber/blob/main/Downloader.md)
  2. [Downloader](https://github.com/podaac/data-subscriber/blob/main/Downloader.md)

In the following tutorial example, we demonstrate access and file extraction of the [**TROPESS CrIS-JPSS1 L2 Carbon Monoxide for Forward Stream, Summary Product V1**](https://disc.gsfc.nasa.gov/datasets/TRPSYL2COCRS1FS_1/summary) dataset. 
