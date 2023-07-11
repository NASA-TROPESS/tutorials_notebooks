# Bulk Data Subscriber and Download Service

This tutorial will demonstrate the utilization of a commandline-based tool known as the **podaac-data-subscriber[downloader]** which allows users to either subscribe to datasets (for periodic, continuous updating featuring the latest available data) or one-time "bulk" downloading of one or more data files with a single request.  

While originally developed by the [PO.DAAC](https://podaac.jpl.nasa.gov/), the **podaac-data-subscriber[downloader]** has recently been upgraded to enable access to data from other NASA Distributed Active Archive Centers (DAACs). For the purposes of this tutorial, we will simply demonstrate data access and extraction of TROPESS data from the NASA GES DISC using the one-time **downloader** feature. 

More specific details regarding the **podaac-data-subscriber[downloader]** can be found here: https://github.com/podaac/data-subscriber

You may also click the following links for more detailed documentation regarding the following options:
  1. [Subscriber](https://github.com/podaac/data-subscriber/blob/main/Downloader.md)
  2. [Downloader](https://github.com/podaac/data-subscriber/blob/main/Downloader.md)

In the following tutorial example, we demonstrate access and file extraction of the [**TROPESS CrIS-JPSS1 L2 Carbon Monoxide for Forward Stream, Summary Product V1**](https://disc.gsfc.nasa.gov/datasets/TRPSYL2COCRS1FS_1/summary) dataset (DOI: [10.5067/JL1HT3NGEAW3](https://doi.org/10.5067/JL1HT3NGEAW3)). 

**Tutorial steps:**
  1. Create an Earthdata Login Account ([clear here for details](https://urs.earthdata.nasa.gov/users/new))
  2. Approve access to the NASA GES DISC Archive in your Earthdata Login Profile ([click here for details](https://disc.gsfc.nasa.gov/earthdata-login))
  3. Create/modify a **.netrc** file in your home directory containing your Earthdata Login credentials as shown below:
     <br>`machine urs.earthdata.nasa.gov login <your username> password <your password>`
  5. Install **podaac-data-subscriber[downloader]** by executing the following 'pip' command from your terminal/commandline:
     <br>`pip install podaac-data-subscriber`
  7. Once installed, run the following command from your commandline:
     <br>`podaac-data-downloader -c TRPSYL2COCRS1FS -d myData -p GES_DISC -sd 2023-06-01T00:00:00Z -ed 2023-07-01T00:00:00Z`

**Explanation of arguments:**
<br>-c Collection name of the queried dataset, specified by the shortname managed by the DAAC.
<br>-d Directory name of the desired location of the data, starting from the current directory of execution.
<br>-p Provider name indicated by the name of the DAAC
<br>-sd Start date/time, in ISO-8601 format
<br>-ed End date/time, in ISO-8601 format

For a more complete explanation of available arguments, you may type the following at your commandline: 
  <br>`podaac-data-downloader --help`

**Expected result:**
A list of 30 files in your specified directory, such as: 
<br>TROPESS_CrIS-JPSS1_L2_Summary_CO_20230601_MUSES_R1p20_FS_F0p6.nc, TROPESS_CrIS-JPSS1_L2_Summary_CO_20230602_MUSES_R1p20_FS_F0p6.nc, etc...
