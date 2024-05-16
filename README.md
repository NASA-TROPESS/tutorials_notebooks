# TROPESS Tutorials & Notebooks

This repo intends to provide a combination of snippet-based tutorials referencing open-source utilities as well as full functioning Jupyter notebooks. 

Tutorials are a work in progress, and will range from any of the following features/capabilities:
1. Data search/discovery
2. Data access/subset/extraction
3. Data plotting/analysis/visualization
4. Direct S3 (Cloud) Access
5. Cloud-based operation

## Special Notes for First-Time Users:
1. See the **[environment.yml](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/environment.yml)** file for a list of dependencies.
2. If you not familiar with managing your own dependencies, we suggest utilizing the provided **[environment.yml](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/environment.yml)** file, as follows:
   
  **Step 1:** Create a new conda environment called tropess-env:
  
   -> Download the **[environment.yml](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/environment.yml)** file.
   
   -> Install Anaconda package: **[https://docs.anaconda.com/free/anaconda/install/](https://docs.anaconda.com/free/anaconda/install/)**
   
   -> Run the following from your commandline: **conda env create --file environment.yml**
   
      
  **Step 2:** Initialize your new "tropess-env" environemnt:
  
   -> Run the following from your commandline: **conda activate tropess-env**
   
   
## Tutorial Summary
| Tutorial Title    | Summary        | Link        | Features/Capabilities |
|-------------------|----------------|-------------|-----------------------|
| Bullk Download of Megacities Data by Species | Demonstrates the utilization of the open-source earthaccess Python library which allows users to query the CMR API for data granule metadata that can then be used for targetted download and extraction via a user-defined temporal bounding box and the gas species. | **[Notebook](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/earthaccess_https_download_megacities_los_angeles.ipynb)** | Data search/access/extraction | 
| Bulk Data Subscriber and Download Service | Demonstrates the utilization of a commandline-based tool known as the podaac-data-subscriber[downloader] which allows users to either subscribe to datasets (for periodic, continuous updating featuring the latest available data) or one-time "bulk" downloading of one or more data files with a single request. | **[Tutorial](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/data_subscriber_downloader.md)** | Data search/access/extraction | 
| TROPESS netCDF Primer Notebook | A Jupyter Notebook coded in Python which fully extracts all data and metadata, then produces a 2-D map plot of the CrIS-JPSS1 L2 Total Column Carbon Monoxide | **[Notebook](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/tropess_primer.ipynb)** | Data extraction/plotting/visualization | 
| Study 2023 Canadian Wildfires using TROPESS CrIS JPSS-1 Carbon Monoxide (CO) data products - **Integrated Data Download** | A Jupyter Notebook coded in Python which reads TROPESS CrIS JPSS-1 CO data products for June 2023 and June 2022 and makes a monthly averaged data product and plots and compare them with fully integrated download of the input data files. | **[Notebook](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/study-2023-canadian-wildfire-effect-integrated_data_download.ipynb)** | Data access/subset/extraction/plotting/analysis/visualization | 
| Study 2023 Canadian Wildfires using TROPESS CrIS JPSS-1 Carbon Monoxide (CO) data products - **Direct S3 (Cloud) Access** | A Jupyter Notebook coded in Python which reads TROPESS CrIS JPSS-1 CO data products for June 2023 and June 2022 directly from S3 on NASA Earthdata Cloud and makes a monthly averaged data product and plots and compare them. | **[Notebook](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/study-2023-canadian-wildfire-effect-integrated_s3access.ipynb)** | Data access/subset/extraction/plotting/analysis/visualization/direct s3 (cloud) access/cloud-based operation |
| Study 2023 Canadian Wildfires using TROPESS CrIS JPSS-1 Carbon Monoxide (CO) data products | A Jupyter Notebook coded in Python which reads TROPESS CrIS JPSS-1 CO data products for June 2023 and June 2022 and makes a monthly averaged data product and plots and compare them. | **[Notebook](https://github.com/NASA-TROPESS/tutorials_notebooks/blob/main/study-2023-canadian-wildfire-effect.ipynb)** | Data plotting/analysis/visualization | 
| Canadian Fires - Carbon Monoxide (CO) - CrIS JPSS-1 | A Jupyter Notebook coded in Python which produces 14x14 km gridded map plots of the Carbon Monoxide (CO) total column for each day from 01-Jun-2023 to 08-Jun-2023. | **[Notebook](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/canadian-fires-gridded-plot-carbon-monoxide-column.ipynb)** | Data plotting/analysis/visualization | 
| Bash Script for Data Download for Canadian Fires - Carbon Monoxide (CO) - CrIS JPSS-1 | Bash script tutorial provides data download for the period from 01-Jun-2023 to 08-Jun-2023. | **[Tutorial/Script](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/canadian-fires-download-data.md)** | Data search/access/extraction | 
| Brazilian Fires - Ammonia (NH3) - CrIS JPSS-1 | A Jupyter Notebook coded in Python which produces 14x14 km gridded map plots of the Ammonia (NH3) total column for each day from from 01-Aug-2022 to 31-Aug-2022. | **[Notebook](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/brazilian-fires-gridded-plot-ammonia-column.ipynb)** | Data plotting/analysis/visualization | 
| Brazilian Fires - Carbon Monoxide (CO) - CrIS JPSS-1 | A Jupyter Notebook coded in Python which produces 14x14 km gridded map plots of the Carbon Monoxide (CO) total column for each day from from 01-Aug-2022 to 31-Aug-2022. | **[Notebook](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/brazilian-fires-gridded-plot-carbon-monoxide-column.ipynb)** | Data plotting/analysis/visualization | 
| Brazilian Fires - PeroxyAcetyl Nitrate (PAN) - CrIS JPSS-1 | A Jupyter Notebook coded in Python which produces 14x14 km gridded map plots of the PeroxyAcetyl Nitrate (PAN) free tropospheric column for each day from from 01-Aug-2022 to 31-Aug-2022. | **[Notebook](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/brazilian-fires-gridded-plot-peroxyacetyl-nitrate-column.ipynb)** | Data plotting/analysis/visualization | 
| Bash Script for Data Download for Brazilian Fires - NH3/CO/PAN - CrIS JPSS-1 | Bash script tutorial provides data download for the period from 01-Aug-2022 to 31-Aug-2022. | **[Tutorial/Script](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/brazilian-fires-download-data.md)** | Data search/access/extraction | 
| Methane (CH4) Partial Column - Scatter Plot | A Jupyter Notebook coded in Python which produces a scatter plot of the Methane (CH4) Partial Column retrieved from the Cross-track Infrared Sounder (CrIS JPSS-1) global observations. | **[Notebook](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/quick-start-scatter-plot-methane-column.ipynb)** | Data plotting/analysis/visualization | 
| Methane (CH4) Partial Column - Gridded Plot (1° x 1°) | A Jupyter Notebook coded in Python which produces a 1° x 1° gridded mapped plot of the Methane (CH4) partial column retrieved from the Cross-track Infrared Sounder (CrIS JPSS-1) global observations. | **[Notebook](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/quick-start-gridded-plot-methane-column.ipynb)** | Data plotting/analysis/visualization | 
| Methane (CH4) Profiles - Scatter Plots | A Jupyter Notebook coded in Python which produces scatter plots at different pressure levels of Methane (CH4) retrieved from the Cross-track Infrared Sounder (CrIS JPSS-1) global observations. | **[Notebook](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/quick-start-scatter-plot-methane-profile.ipynb)** | Data plotting/analysis/visualization | 
| Carbon Monoxide Column (XCO) | A Jupyter Notebook coded in Python which column variable x_col a.k.a. XCO, in ppbv. The XCO is a pre-calculated vertically averaged dry air mixing ratio of carbon monoxide from the surface to Top of Atmosphere (TOA). CO concentrations are retrieved from CrIS JPSS-1 global observations. | **[Notebook](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/data-analysis-carbon-monoxide-plot-column-xvmr.ipynb)** | Data plotting/analysis/visualization | 
| Bash Script for Data Download for Methane (CH4) from CrIS JPSS-1 | Bash script tutorial provides data download for CH4 retrievals on 16-May-2023. | **[Tutorial/Script](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/quick-start-download-data.md)** | Data search/access/extraction | 
| Running in Google Colab | Google Colaboratory (Colab) is an alternate cloud-based environment to run Jupyter notebooks, with lots of additional features, like GPUs, storage in Github or Google Drive, and access to Google Cloud. | **[Tutorial/Script](https://github.com/NASA-TROPESS/tropess-notes/blob/main/book/how-to-run-google-colab.md)** | cloud-based operation | 
| Homepage for TROPESS Tutorials and Notebooks from Swift Software Group | Assorted Jupyter notebooks for TROPESS data access and analysis. | **[Notebooks/Tutorials](https://github.com/NASA-TROPESS/tropess-notes/)** | Data access/subset/extraction/plotting/analysis/cloud-based operation | 
| Python-based Repository for TROPESS Tutorials and Notebooks from Swift Software Group | Assorted Jupyter notebooks for TROPESS data access and analysis. | **[Notebooks/Tutorials](https://github.com/NASA-TROPESS/tropess-notes-python/)** | Data access/extraction/plotting/analysis/cloud-based operation | 
| GES DISC Tutorials | GitHub Repo with Jupyter Notebooks and Tutorials | **[External Tutorials and Notebooks](https://github.com/nasa/gesdisc-tutorials)** | Data search/discovery/access/subset/extraction/plotting/analysis/visualization |

## Copyright and Licensing Info
Copyright (c) 2023-24 California Institute of Technology (“Caltech”). U.S. Government sponsorship acknowledged. All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided
that the following conditions are met:

• Redistributions of source code must retain the above copyright notice, this list of conditions and
the following disclaimer.

• Redistributions in binary form must reproduce the above copyright notice, this list of conditions
and the following disclaimer in the documentation and/or other materials provided with the
distribution.

• Neither the name of Caltech nor its operating division, the Jet Propulsion Laboratory, nor the
names of its contributors may be used to endorse or promote products derived from this software
without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS
IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR
CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

Open Source License Approved by Caltech/JPL
APACHE LICENSE, VERSION 2.0
• Text version: https://www.apache.org/licenses/LICENSE-2.0.txt
• SPDX short identifier: Apache-2.0
• OSI Approved License: https://opensource.org/licenses/Apache-2.0
