# LarkData - Alouette I Ionogram Search Engine and Custom Ionogram Image Metadata Processing Algorithms
###### Spaceapps Toronto 2017 Hackathon
###### CSA Challenge #1: "Be part of Canada's legacy in space!"

<div style="text-align:center"><a href="http://larkdata.space/"><img src ="http://i.imgur.com/VSdbx3U.jpg" /></a></div>

#TEMPORARY PLACEHOLDER<br />
#TO BE REVAMPED WITH MORE INFORMATION/POLISHED COPY<br />

## Links to Live Website:
http://larkdata.space<br />
http://lark-data.space<br />
http://larkdata.heliohost.org<br />

## Video of Our Presentation at SpaceApps Toronto 2017
[![SpaceApps Toronto 2017 Presentations](http://i.imgur.com/wxEdpt9.png)](https://www.youtube.com/watch?v=U5yd2ZN50Yk&feature=youtu.be&t=1h31m35s "SpaceApps Toronto 2017 Presentations")

## Team Members (Credits):
* Ali Karamali<br />
* Amy Yi<br />
* Erin Hong<br />
* Frederic Pun @fpunny<br />
* Huanning Wang<br />
* Jim Rootham @jrootham<br />
* Karlille John @KarlilleJohn<br />
* Michelle Villar<br />
* Mohammad Ismail @ismailmohammad<br />
* Patrick Ocampo<br />
* Prashant Patel @prasvpatel<br />
* Sameed Sohani @asonance<br />

## How to Navigate this Repository (Additional Information):
This repository is divided up into the various components that are required to either replicate the project we have created locally or to be hosted online. Below is a guide to uncomplicate perhaps the somewhat complicated but explanatory directories.
### LarkData Hackathon Localhost Files:
This directory contains the original files from the demo used at the Space Apps Toronto 2017 Hackathon, including the obsolete and/or unnecessary files to maintain the integrity of the project files and display them as we had it at the time of the deadline. If needed to recreate this, please place the files within this directory within the XAMPP htdocs or the general root location of your local server.
### LarkData LiveWebsite Files:
This directory within the repo contains the actual required files needed to host our project online along with its coded sample PostgreSQL database hosted on ElephantSQL. The code within result.php can be modified with your own database credentials. The files within this directory is also a revamp of the Weekend project with an updated header. The site at the moment is intended for Desktop users, considering our target audience. Also another change within this source code is that the images within the img folder have been compressed into .JPG format, bringing down the entire size of the directory to about ~30 MB allowing for quick viewing of images with the option to download the full resolution TIFF images (roughly 30-40 MB each) from the offical ftp Server.
### PHP Extensions to Ensure Enabled:
This is regarding if website is hosted locally, or if online and you have full control of your server. This directory contains is the instructions to enable the PHP extensions php_pdo_pgsql.dll and php_pgsql.dll enabling PHP support for PostgreSQL databases and the use of various functions such as pg_connect(); that are necessary for the successful operation of our tool. Our initial choice for hosting did not have PHP PostgreSQL enabled and neither did XAMPP by default so this is to assist users.
### PostgreSQL Setup Scripts:
This directory contains the scripts necessary to set up the local PostgreSQL database, with its respective tables. The sample_data.CSV can be replaced with a larger set of data generated by our Python Image Metadata Processing Algorithms. One note however, should you not have full superuser privileges of a database to COPY from local files, You may use a CSV to SQL converter to convert the CSV in question into a list of SQL insert commands such as <a href="http://www.convertcsv.com/csv-to-sql.htm"></a>. We are not affiliated with the aforementioned website in any way.
### Presentation - Sunday April 30th, 2017:
This directory simply contains a .ppt version of the presentation used at the SpaceApps Toronto 2017 Presentation and also a link to the actual Google Slides presentation used as well.
### Python Image Processing and CSV generating Algorithms:
This directory contains the the python programs we created over the weekend to parse the Allouette images in their original .tif format for their metadata and to determine if the Ionogram does infact have valid metadata as there were instances of blank images or just metadata without their related image.
### Sample Data Sets:
Lastly, this directory contains the station_location.CSV and sample_data_old_witherrors.CSV which were used at the actual presentation. However the new sample_data.CSV and sample_data (USE THIS ONE...).CSV were also included to provide the most accurate data for our live demo on the websites.
